# MATLAB & Simulink Agentic Toolkit Offline Installation

Install the MATLAB and Simulink Agentic Toolkits and MATLAB MCP Server on an offline or air-gapped PC using the Installer App. Simulink workflows require MATLAB R2023a or later and a Simulink license.

## Quick Start

1. On an internet-connected PC, download **`agentic-offline.zip`** and **`AgenticToolkitOfflineInstallerApp.m`** from [GitHub Releases](https://github.com/JongnamKim/MATLAB-Simulink-Agentic-Toolkit-Offline-Installation/releases). The ZIP includes the MCP server binary, MCP toolbox, and MATLAB/Simulink Toolkits.
2. Extract the ZIP (for example, to `D:\agentic-offline`) and transfer the extracted folder together with the App file to the offline PC.
3. In MATLAB, set the current folder to the App file's location and run:

   ```matlab
   AgenticToolkitOfflineInstallerApp
   ```

4. Set **Offline Package Folder** to the extracted folder, select **MATLAB**, **Simulink**, or **MATLAB and Simulink**, then click **Install Offline**.
5. Select the required **Skill Groups**, click **Install Skills**, then **Status / Initialize**.

## Share the MATLAB Session at Startup

Run `which('startup', '-all')` and edit the first `startup.m` listed. If none exists, create one with `edit(fullfile(userpath, 'startup.m'))`. Preserve existing content and add **one** of the following options.

**MATLAB Toolkit only:**

```matlab
shareMATLABSession()
```

**Simulink Toolkit, or both Toolkits:**

```matlab
if ispc
    addpath(fullfile(getenv('USERPROFILE'), '.matlab', 'agentic-toolkits', 'simulink'))
else
    addpath("~/.matlab/agentic-toolkits/simulink")
end
satk_initialize
```

These are installed Toolkit paths; adjust them if you used a different installation location. `satk_initialize` already calls `shareMATLABSession`, so no additional sharing call is needed. Restart MATLAB after saving `startup.m`.

## Configure the Agent and Verify

Use an MCP-capable AI agent connected to your internal LLM endpoint. The HTML guide uses **Roo Code** as an example.

For Windows, set the MCP server command to `C:/Users/<user>/.matlab/agentic-toolkits/bin/matlab-mcp-server.exe` and configure its arguments:

- `--matlab-session-mode=existing`: connect to the shared, running MATLAB session.
- `--extension-file=C:/Users/<user>/.matlab/agentic-toolkits/simulink/tools/tools.json`: load Simulink tools when using Simulink.

Replace `<user>` with your account name and adjust paths for your installation. In MATLAB, run:

```matlab
setupAgenticToolkit("status")
mcpSessionCheck = "airgap-session-check";
```

Ask the agent to read `mcpSessionCheck`, confirm its value, and report the MATLAB version. If a Simulink model is open, also ask it to describe the model's structure and signal flow.

## Related Resources

- [Detailed HTML installation guide](../Agentic%20Toolkit%20Installation%20Guidance/Air_gapped_agentic_toolkit_installation_guide.html)
- [MATLAB Agentic Toolkit](https://github.com/matlab/matlab-agentic-toolkit/)
- [Simulink Agentic Toolkit](https://github.com/matlab/simulink-agentic-toolkit/)

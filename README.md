# MATLAB & Simulink Agentic Toolkit Offline Installation

This repository provides resources for installing the MATLAB Agentic Toolkit, Simulink Agentic Toolkit, and MATLAB MCP Server in offline or air-gapped environments.

## Why This Repository Is Needed

An offline PC cannot download installation files directly from online sources. The required packages must first be prepared on an internet-connected PC, transferred to the target environment, and installed from local files.

This repository brings together the installation package, Installer App, and HTML guide to support that process. Versioned releases help keep these resources aligned, while the Installer App automates the installation work on the offline PC. This README introduces the overall workflow; the HTML guide provides the detailed instructions.

## Installation Resources

Download the **HTML installation guide, Installer App, and installation files** together from [GitHub Releases](https://github.com/JongnamKim/MATLAB-Simulink-Agentic-Toolkit-Offline-Installation/releases).

| Resource | Purpose |
| --- | --- |
| HTML installation guide | Explains prerequisites, Installer App usage, agent configuration, MATLAB session sharing, and verification. |
| Installer App (`AgenticToolkitOfflineInstallerApp.m`) | Automates installation of the selected Toolkit and MCP components from local files. |
| Installation package (`agentic-offline.zip`) | Contains the MCP server binary, MCP toolbox, MATLAB/Simulink Toolkits, and supporting installation files. |

Use the guide, App, and package supplied for the same release. Refer to the release information and HTML guide for supported operating systems and MATLAB versions.

## Offline Installation Workflow

**Prepare → Download → Transfer → Install → Connect → Verify**

1. **Review the target environment.** Read the HTML guide and confirm the target OS, MATLAB release, required products and licenses, and available AI agent.
2. **Prepare the installation resources.** On an internet-connected PC, download the three resources from the selected release and extract the installation package. Prepare the files needed for the target platform.
3. **Transfer to the offline PC.** Move the extracted folder together with the Installer App and HTML guide using your organization's approved transfer method. Preserve the package's folder structure.
4. **Install with the Installer App.** Run the App in MATLAB on the offline PC to install the required Toolkit and MCP components. Follow the HTML guide for the App's operation and installation settings.
5. **Configure the connections.** Set up the AI agent's connection to the internal LLM and the MATLAB MCP Server. Refer to the HTML guide for agent configuration and MATLAB session sharing, including startup automation.
6. **Verify the installation.** Follow the HTML guide to confirm that the agent can access the intended MATLAB session and, when applicable, work with Simulink models. Retain the release information for future maintenance or reinstallation.

## Related Resources

- [MATLAB Agentic Toolkit](https://github.com/matlab/matlab-agentic-toolkit/)
- [Simulink Agentic Toolkit](https://github.com/matlab/simulink-agentic-toolkit/)

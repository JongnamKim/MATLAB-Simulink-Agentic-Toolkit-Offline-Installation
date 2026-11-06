# MATLAB & Simulink Agentic Toolkit Offline Installation

This repository provides installation packages, an Installer App, and an HTML guide for deploying the MATLAB and Simulink Agentic Toolkits with the MATLAB MCP Server in offline or air-gapped environments.

## Installation Workflow

**Prepare → Download → Transfer → Install → Connect → Verify**

1. **Prepare:** Review the [HTML installation guide](../Agentic%20Toolkit%20Installation%20Guidance/Air_gapped_agentic_toolkit_installation_guide.html) and confirm the target OS, MATLAB compatibility, and required products.
2. **Download:** On an internet-connected PC, obtain the offline package and Installer App from [GitHub Releases](https://github.com/JongnamKim/MATLAB-Simulink-Agentic-Toolkit-Offline-Installation/releases), then extract the package.
3. **Transfer:** Check any supplied checksums and transfer the extracted folder together with the Installer App to the offline PC using your organization's approved method.
4. **Install:** Use the Installer App on the offline PC to install the required Toolkit components.
5. **Connect:** Configure the AI agent, internal LLM access, and MATLAB MCP session connection.
6. **Verify:** Confirm that the agent can access the intended MATLAB session and, when applicable, Simulink models.

Refer to the **HTML installation guide** for detailed Installer App usage, installation settings, session sharing, agent configuration, and verification instructions.

## Related Resources

- [MATLAB Agentic Toolkit](https://github.com/matlab/matlab-agentic-toolkit/)
- [Simulink Agentic Toolkit](https://github.com/matlab/simulink-agentic-toolkit/)

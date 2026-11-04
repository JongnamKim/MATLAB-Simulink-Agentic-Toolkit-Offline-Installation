# MATLAB \& Simulink Agentic Toolkit Offline Installation

This repository provides installation resources and documentation for installing the MATLAB Agentic Toolkit and Simulink Agentic Toolkit in offline or air-gapped environments.

The repository is intended to support the preparation, management, transfer, installation, and verification of the required packages when the target computer does not have internet access.

## Quick Start

1. Review the HTML installation guide in **Agentic Toolkit Installation Guidance**.
2. Download the required installation package from **GitHub Releases**.
3. Transfer the downloaded files to the offline PC using your organization's approved transfer method.
4. Launch the installation app from **Agentic Toolkit Installation Apps**.
5. Follow the app instructions to install the required components.
6. Verify the installation by following the verification steps in the HTML guide.

## 1\. Overview

This repository contains installation-related resources for:

* MATLAB Agentic Toolkit
* Simulink Agentic Toolkit
* MATLAB MCP Server
* Supporting installation applications and guidance

The required installation packages are prepared or downloaded on an internet-connected PC and then transferred to the offline PC when required.

### Component Roles

|Component|Purpose|
|-|-|
|README|Provides an overview and quick-start workflow.|
|HTML Installation Guide|Provides detailed offline installation, configuration, and verification guidance.|
|Installation App|Automates installation steps on the target offline PC.|
|GitHub Releases|Provides versioned installation packages and supporting files for download.|
|Checksum File|Enables integrity verification of transferred installation files when provided with a release.|

## 2\. Repository Contents

|Folder / File|Description|
|-|-|
|`Agentic Toolkit Installation Apps`|Installation applications used to automate the offline installation workflow.|
|`Agentic Toolkit Installation Guidance`|HTML installation guides and supporting documentation.|
|`Agentic Toolkit Offline Installation Files`|Files and supporting resources required for offline installation.|
|`README.md`|Repository overview, quick-start instructions, and package information.|

## 3\. Recommended Offline Installation Workflow

### Step 1 - Review the Installation Guide

Open the HTML installation guide and review the prerequisites, required files, installation sequence, and verification procedure before transferring files to the offline environment.

### Step 2 - Download the Installation Package

Download the installation package and supporting assets from the appropriate GitHub Release.

When multiple releases are available, use the release that matches the intended MATLAB release and installation guide.

### Step 3 - Verify the Downloaded Files

If a SHA-256 checksum file is included in the release, verify the downloaded files before transferring them to the offline environment.

This step is recommended to confirm that the installation files have not changed during download or transfer.

### Step 4 - Transfer Files to the Offline PC

Transfer the installation package to the offline or air-gapped PC using an approved file-transfer method for the target environment.

Keep the package structure unchanged unless the corresponding installation guide explicitly requires a different directory layout.

### Step 5 - Run the Installation App

Launch the provided MATLAB installation app and follow its instructions to install the required toolkit components.

The installation app is intended to automate the installation workflow and reduce the number of manual installation steps.

### Step 6 - Verify the Installation

After installation, follow the verification procedure in the HTML installation guide to confirm that the required MATLAB and Simulink Agentic Toolkit components are available and configured as expected.

## 4\. GitHub Releases

Installation packages are distributed through GitHub Releases so that installation resources can be managed by version.

A release may contain the following assets, depending on the toolkit version and installation requirements:

* Offline installation ZIP package
* Required executable files
* MATLAB Toolbox installation files
* Supporting installation files
* Installer app
* HTML installation guide
* SHA-256 checksum file
* Release notes

### Recommended Release Information

Each release should clearly identify:

* Release version
* Supported MATLAB release or releases
* Included Agentic Toolkit components
* Installation guide version
* Known limitations or special installation requirements
* SHA-256 checksums for downloadable installation assets, when provided

Keeping the release, installation guide, and installation app versions aligned helps make the offline installation package reproducible and easier to maintain.

## 5\. Version and Compatibility Information

|Item|Information|
|-|-|
|Repository|MATLAB \& Simulink Agentic Toolkit Offline Installation|
|Release|See the applicable GitHub Release.|
|Environment|Windows / Offline or air-gapped environment|
|MATLAB Compatibility|Confirm compatibility in the applicable release notes and installation guide.|

Because toolkit requirements can change between versions, confirm that the selected release, installation guide, and target MATLAB release are compatible before installation.

## 6\. File Integrity

For offline and air-gapped deployments, file-integrity verification is recommended when checksum information is provided with the release.

A SHA-256 checksum file can be used to verify that files downloaded on the internet-connected PC are identical to the files transferred to the offline PC.

Keep checksum information together with the corresponding release so that each installation package can be verified independently.

## 7\. Notes and Recommendations

* Verify that all required installation files are available before transferring them to the offline PC.
* Confirm compatibility with the target MATLAB release and operating system.
* Keep installation packages, the installer app, and documentation organized by release version.
* Use the HTML installation guide as the detailed installation reference and this README as the repository overview and quick-start entry point.
* Avoid changing the directory structure of an installation bundle after it has been validated for offline installation.
* Do not include passwords, API keys, access tokens, licenses, or other sensitive credentials in this repository or its releases.

## 8\. Intended Workflow at a Glance

**README -> HTML Guide -> GitHub Release -> File Transfer -> Installation App -> Verification**

The README provides the starting point, the HTML guide explains the detailed procedure, GitHub Releases provide the required installation packages, and the installation app automates the installation on the offline PC.


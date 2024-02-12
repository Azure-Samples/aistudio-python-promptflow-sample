# 1. Setup Dev Environment

To get started quickly, you can use a pre-built development environment. 
**Click the button below** to open the repo in GitHub Codespaces, and then continue the readme!

[![Open in GitHub Codespaces](https://github.com/codespaces/badge.svg)](https://codespaces.new/Azure-Samples/aistudio-python-promptflow-sample?quickstart=1?WT.mc_id=academic-112432-pablolopes)

For other options, continue with the instructions.
If you used Codespaces, we can now [_create our AI Project resource_](./02-create-aiproject.md).

## 1.1 Pre-Requisites

**Required:**

- A GitHub account | 👉🏽 [Signup for GitHub](https://github.com/signup?WT.mc_id=academic-112432-pablolopes) 
- An Azure account | 👉🏽 [Signup for Azure](https://azure.microsoft.com?WT.mc_id=academic-112432-pablolopes)
- An active Azure subscription that
    - has Microsoft.MachineLearningService resource provider registered (should be by default)
    - is enrolled in AI Studio Private Preview 
    - is allow-listed for Azure OpenAI Service (if used)

**Optional:**

- Set of docs copilot can use for Q&A - else use [sample data](./../data/).
- GitHub Codespaces for prebuilt dev environment - else install manually


## 1.2. Pre-Built Dev Environment

Our pre-built development environments use the concept of [dev containers](https://containers.dev?WT.mc_id=academic-112432-pablolopes) to provide a consistent and reproducible development environment for _all_ users of the project. 

The dev container uses a _configuration-as-code_ approach, using a [devcontainer.json](./../.devcontainer/devcontainer.json?WT.mc_id=academic-112432-pablolopes) file that can be checked-in and version-controlled alongside the code. It currently uses:
 - [this Python 3.10 image](https://mcr.microsoft.com/en-us/product/devcontainers/python/about?WT.mc_id=academic-112432-pablolopes) as the base container
 - [this Dockerfile](./../.devcontainer/Dockerfile?WT.mc_id=academic-112432-pablolopes) for additional customizations

You can _launch_ the development environment in two ways:
 - using GitHub Codespaces in the cloud (**recommended**)
 - using Docker Desktop on your local device

We'll walk through both options below. Note that in either case, any changes to the environment configuration (e.g., change to `devcontainer.json`, `requirements.txt` or `.env`) **will require a rebuild of the container** to take effect.

### 1.2.1 Launch GitHub Codespaces

To get started with GitHub Codespaces, fork this sample repository to your GitHub profile - then use the `Code` drop-down menu to select the `Codespaces` tab and click the **Create codespace** as shown.

![Create Codespaces](../img/00-DeployCodespaces.png?WT.mc_id=academic-112432-pablolopes)

This should open a new tab in your browser and start building the development container for your project.

![Launch Codespaces](../img/01-DeployingCodespaces.png?WT.mc_id=academic-112432-pablolopes)

Once completed, the tab should refresh to show you a Visual Studio Code editor in the browser, as shown below.

![Visual Studio Code Editor](../img/02-CodespaceDeployed.png?WT.mc_id=academic-112432-pablolopes)

**Note:** The blue tab in the status bar (bottom left) reflects the current status of your dev container, showing it is currently using GitHub Codespaces. Click the tab to open a menu with options to rebuild, reconfigure, or reconnect to, this Codespaces instance.

![Visual Studio Code Editor](../img/03-BottomLeftCodespacesOption.png?WT.mc_id=academic-112432-pablolopes)

![Codespaces Options](../img/04-MenuDevContainers.png?WT.mc_id=academic-112432-pablolopes)


> [!NOTE]
> 🎉 **Congratulations**. Your development environment is ready for use in GitHub Codespaces!

### 1.2.2 Launch Docker Desktop

Using GitHub Codespaces is the fastest and most reliable way to launch the development environment. However, you may want to setup a _local development environment_ for some contexts - e.g., to work offline.

Fortunately, you should be able to use the _same_ development container configuration with **Docker Desktop**  on your local device as follows.

1. Clone the repo to your local device, then open it in a Visual Studio Code editor as usual. Because your repository has a `.devcontainer` configuration, you may automatically see a pop-up like this asking if you want to _"Reopen in Container"_.
    ![Reopen in Container](../img/05-OpenLocalDevice.png?WT.mc_id=academic-112432-pablolopes)

2. Make sure you have Docker Desktop installed and running first. This is what that dashboard looks like.
    ![Docker Desktop](../img/06-DockerDesktop.png?WT.mc_id=academic-112432-pablolopes)

3. If you don't see the pop-up or it has disappeared (after a timeout), simply click the blue `><`icon (bottom left of status bar) for menu options and select _"Reopen in Container"_.
    ![Reopen in Container](../img/07-ReopenContainer.png?WT.mc_id=academic-112432-pablolopes)

4. This should now begin the process of starting the development container in the Docker Desktop - including downloading required images and installing specified dependencies. _This may take some time for the initial setup, but subsequent usage will be quicker_.
    ![Reopen in Container](../img/08-StartContainer.png?WT.mc_id=academic-112432-pablolopes)

5. Once container setup is complete, you should see the Docker Desktop showing you the running container in its Dashboard "Containers" panel.
    ![Reopen in Container](../img/09-RunningContainer.png?WT.mc_id=academic-112432-pablolopes)
    
6. The Visual Studio Code editor should now show an updated DevContainer widget (bottom left of status bar) with a label like `Dev Container: ..` (as opposed to `Codespaces..`) - which gives you a visual cue about _which_ dev container environment you are connected to (local vs. cloud).
    ![Reopen in Container](../img/10-ViewVSCode.png?WT.mc_id=academic-112432-pablolopes)

> [!NOTE]
> 🎉 **Congratulations**. Your development environment is ready for use in Docker Desktop!


## 1.4 Next Steps

At this point you have a working development environment with the Azure AI CLI installed and ready to use. We can now [_create our AI Project resource_](./02-create-aiproject.md?WT.mc_id=academic-112432-pablolopes).

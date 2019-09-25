# NUnit.org website

To get started developing the website, you have two options. You can develop in a Docker Container using VS Code, or you can install Ruby locally and develop locally.

## Installing Docker and VS Code

Do this if you want to develop in a Docker container using VS Code.

1. Install and configure [Docker](https://www.docker.com/get-started) for your operating system.

    **Windows / macOS**:

    1. Install [Docker Desktop for Windows/Mac](https://www.docker.com/products/docker-desktop).
    2. Right-click on the Docker taskbar item and update **Settings / Preferences > Shared Drives / File Sharing** with the drive the web app source code is located in. If you run into trouble, see [Docker Desktop for Windows tips](/docs/remote/troubleshooting.md#docker-desktop-for-windows-tips) on avoiding common problems with sharing.

    **Linux**:

    1. Follow the [official install instructions for Docker CE/EE for your distribution](https://docs.docker.com/install/#supported-platforms).
    2. Add your user to the `docker` group by using a terminal to run: `sudo usermod -aG docker $USER`
    3. Sign out and back in again so your changes take effect.

2. Install [Visual Studio Code](https://code.visualstudio.com/).
3. Install the [Remote Development extension pack](https://aka.ms/vscode-remote/download/extension).

### Quick Start for Docker with VSCode

1. Start VS Code and click on the quick actions Status Bar item in the lower left corner of the window.

    ![Quick actions status bar item](https://code.visualstudio.com/assets/docs/remote/common/remote-dev-status-bar.png)

2. Select **Remote-Containers: Open Folder in Container...** from the command list that appears, and open the root folder of the project you just cloned.

3. The window will then reload, but since the container does not exist yet, VS Code will create one. This may take some time, and a progress notification will provide status updates. Fortunately, this step isn't necessary the next time you open the folder since the container will already exist.

    ![Dev Container Progress Notification](https://code.visualstudio.com/assets/docs/remote/containers/dev-container-progress.png)

4. After the container is built, VS Code automatically connects to it and maps the project folder from your local file system into the container.

5. Open the terminal in VS Code to a bash prompt within the container by clicking on **Terminal > New Terminal**

6. In the terminal, type `bundle exec jekyll serve` to build and run the web site. (See below)

7. Open the web site at [http://localhost:4000](http://localhost:4000).

8. Begin developing in Visual Studio Code.

## Installing Ruby and Jekyll locally

1. Install Ruby 2.2 ([Linux](https://www.ruby-lang.org/en/documentation/installation/), [Mac](https://gorails.com/setup/osx/10.10-yosemite), [Windows](http://rubyinstaller.org/))
2. If you are on Windows, install [DevKit](http://rubyinstaller.org/add-ons/devkit/)
3. `gem install bundler`
4. `bundle install`

## Building the project

GitHub will do this automatically when you push, but this allows you to view the site locally before you commit.

1. `jekyll serve`
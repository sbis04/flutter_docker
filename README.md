# Dockerizing Flutter apps

![Flutter Docker cover](https://i.imgur.com/wy6vrUU.png)

[Docker](https://www.docker.com/) helps to **simplify** and **accelerate** the development workflow, while giving the freedom to choose any **tool** and maintain different development **environments** for each project.

#### Check out my article on **Codemagic Blog** for detailed guide, [here](https://blog.codemagic.io/how-to-dockerize-flutter-apps/).

## Prerequisites

* Make sure you have [Docker](https://docs.docker.com/engine/install/) properly setup on your system.
* [VS Code](https://code.visualstudio.com/) along with two extensions [Docker](https://marketplace.visualstudio.com/items?itemName=ms-azuretools.vscode-docker) & [Remote Development](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.vscode-remote-extensionpack).

## Using the container

This repository contains a basic **Flutter Docker Container** setup. You can add additional tools as per your requirements in the **Dockerfile**. Also, one **demo** Flutter project is present in the `workspace` folder which you can build and run in the **Docker Container**.

The steps for using this Docker Container are as follows:

1. Clone this repo:
   ```bash
   git clone https://github.com/sbis04/flutter_docker.git
   ```

2. Open this project directory using **VS Code**:
   ```bash
   code flutter_docker
   ```

3. Click on the **Remote Development icon** (present in the bottom-left corner of VS Code).

4. Select the option **Remote-Containers: Open Folder in Container** from the list.

5. Select the root directory which contains the **Dockerfile** (along with some other settings) and click on **Open** to start building the Docker container. This will take some time as it will download and setup all the tools in the container.

6. After the build finishes, you will be taken to the **bash terminal** of the **Docker container**.

7. Now, you can **build**, **test** and **run** Flutter apps in the container.

# License

Copyright (c) 2020 Souvik Biswas

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.

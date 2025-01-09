# Docker XAMPP with XDebug Sample
___

A docker-compose.yml file is provided to bring up an XAMPP PHP Development environment for the purpose of learning PHP.  **This configuration is not intended to be used as a production environment**.

## Getting Started

___

- Prerequisite: Installation of Docker Desktop
- You may use Visual Studio's terminal window, Windows PowerShell or macOS Terminal window to run the following docker command to bring up the docker environment.
  - Navigate to the directory that contains the GitHub repo for the XAMPP with Debug local repository in a terminal or a powershell window.
  - Change directory to the docker directory, i.e., "cd docker".
  - The first time we bring up the container, the apache image will be pulled and built with PDO, XDebug, etc., so we must execute add a parameter that will not be required after the image is built.  Execute the following command to build bring up the containers and build the initial apache container: "docker-compose up --build -d".
  - To shut down the containers, you can either stop them in Docker Desktop or execute the following command to bring the containers down: "docker-compose down".
  - Any subsequent times you want to bring up the container assuming that you have not removed any of the created images or volume, you can execute the following command: "docker-compose up -d".

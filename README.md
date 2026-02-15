# [Optimization and Learning for Robot Control]

Optimization and Learning for Robot Control Lecture with Slides, Codes and Youtube.

## 📺 Overview
This repository provides Korean-language lecture videos based on the optimization and learning curriculum. 
This course covers fundamental inverse kinematics and dynamics control, optimization based control and learning based control for robotics engineering.

* **Youtube Playlist**: https://www.youtube.com/playlist?list=PLjHPb6Q6WLfJdX5vqrljsbdVw6JXkZmcV

---

## 🐳 Installation using Docker

Docker provides a consistent environment for all students regardless of their operating system (Linux, Windows WSL2, or Mac).

### 1. Prerequisites

Before we begin, please ensure you have the following installed:

* **Docker Desktop**: https://www.docker.com/products/docker-desktop/
* **Visual Studio Code (VS Code)**: https://code.visualstudio.com/
* **VS Code Extensions**:
    * Docker
    * Dev Containers

### 2. Download the Lab Environment

Open your terminal (PowerShell, CMD, or Terminal) and download the pre-configured robot control image:

> docker pull rcilab/robot_control:v1

### 3. Running the Container (Recommended Workflow)

We recommend using VS Code Attach mode for the best development experience.

#### Step 1: Start the container
Run the following command in your local terminal to start the environment in the background:

> docker run -it -d --rm --name orc_lab rcilab/robot_control:v1

#### Step 2: Attach VS Code
1. Open VS Code.
2. Click the Docker icon on the left sidebar (Activity Bar).
3. Under the CONTAINERS section, find 'orc_lab'.
4. Right-click on 'orc_lab' and select "Attach Visual Studio Code".
5. A new window will open. You are now working inside the container!

#### Step 3: Verify the Setup
Inside the attached VS Code terminal (Ctrl + `), run:

> python3 -c "import orc; print('SUCCESS: Environment is ready!')"

### 💡 Tips for Students

* Plotting: GUI windows do not open in Docker. Use 'plt.savefig('my_plot.png')' to save results as images and view them in the VS Code file explorer.
* Saving Work: Since we used the '--rm' flag, the container is deleted when stopped. Make sure to backup your code!
* Stopping: To shut down the environment, run 'docker stop orc_lab' in your local terminal.


## Contact
Maintainer: [Sanghyun Kim] (kim87@khu.ac.kr)  
Lab: [RCI Lab @ Kyung Hee University](https://rcilab.khu.ac.kr)


1&emsp;About Part 2 Project
==============

***EE3305/ME3243 Robotic System Design***

**&copy; National University of Singapore**

Implement Dijkstra path planning and Pure Pursuit controller to move a Turtlebot3 robot in a simulated environment.

The project is coded using ROS2 Jazzy, and either Python or C++ can be used.

# Table of Contents

[1&emsp;Overview](#1overview)

[2&emsp;Install Ubuntu and ROS2](#2install-ubuntu-and-ros2)

[3&emsp;Setup Project](#3setup-project)

[4&emsp;Tasks](#4tasks)

# 1&emsp;Overview
<table><tbody>
    <tr>
        <td><b>Effort</b></td>
        <td colspan="2">Teams of 3</td>
    </tr>
    <tr>
        <td><b>Deadline</b></td>
        <td colspan="2">All submittables by 9 Nov 2025 (W12 Sun) 23:59h.</td>
    </tr>
    <tr>
        <td rowspan="3"><b>Submittables</b></td>
        <td><b>P2C</b></td>
        <td>
            <ul>
                <li>30% of the project score.</li>
                <li><code>.zip</code> file of the workspace directory <b>containing only</b> the <code>src</code> directory. To avoid penalties, the top level of the zip file contains only the <code>src</code> directory, and the zip file should not exceed 1MB.</li>
                <li>The code should be executable and buildable without errors.</li>
            </ul>
        </td>
    </tr>
    <tr>
        <td><b>P2P</b></td>
        <td>
            <ul>
                <li>30% of the project score.</li>
                <li><code>.pdf</code> A3 poster succinctly describing any outstanding improvements or analysis in the project.</li>
                <li>The poster is presented online during the allocated presentation slot.</li>
                <li>During the presentation, members must describe personal contributions including improvements and analysis when asked to do so by assessors.</li> 
                <li>The poster allows assessors to form an impression of the team effort so that more advanced questions can be asked. Answering them adequately will lead to more marks.</li>
                <li>The poster will be checked for plagiarism using Turnitin.</li>
            </ul>
        </td>
    </tr>
    <tr>
        <td><b>P2R</b></td>
        <td>
            <ul>
                <li>40% of the project score.</li>
                <li><code>.pdf</code> report focusing on the tuning methodologies, observations, explanations, and suggestions. Improvements should also be described.</li>
                <li>About 10 to 15 pages excluding front and back matter. There are no hard constraints on the number of pages.</li>
                <li>The report will be checked for plagiarism using Turnitin.</li>
            </ul>
        </td>
    </tr>
    <tr>
        <td><b>Software</b></td>
        <td colspan="2">Ubuntu 24.04 and ROS2 Jazzy. See below for installation steps.</td>
    </tr>
</tbody></table>

# 2&emsp;Install Ubuntu and ROS2
Install Ubuntu 24.04 and ROS2 Jazzy based on the following guides. 

Ubuntu 24.04 can be installed on VirtualBox (virtualization) or dual boot are supported. 
If your computer has warranty and you have backed up your data, dual booting is strongly recommended.
Doing so allows you to learn about the process and the steps to solve any errors that occur.
Otherwise, VirtualBox can be used.

<table><tbody>
    <tr>
        <th>Guide</td>
        <th>Description</td>
    </tr>
    <tr>
        <td><a href="https://github.com/LaiYanKai/Misc/blob/main/rb2301/01_Where_To_Install_Ubuntu.md">01_Where_To_Install_Ubuntu.md</a></td>
        <td>The steps to prepare for Ubuntu installation depending on where Ubuntu will be installed.</td>
    </tr>
    <tr>
        <td><a href="https://github.com/LaiYanKai/Misc/blob/main/rb2301/02_Getting_Ubuntu.md">02_Getting_Ubuntu.md</a></td>
        <td>Prepares for the installation of Ubuntu depending on where it would be installed.</td>
    </tr>
    <tr>
        <td><a href="https://github.com/LaiYanKai/Misc/blob/main/rb2301/03_Installing_Ubuntu.md">03_Installing_Ubuntu.md</a></td>
        <td>Installs Ubuntu.</td>
    </tr>
    <tr>
        <td><a href="https://github.com/LaiYanKai/Misc/blob/main/rb2301/04_Installing_Ubuntu_Software.md">04_Installing_Ubuntu_Software.md</a></td>
        <td>Installs software such as Visual Studio Code and ROS2 on Ubuntu.</td>
    </tr>
</tbody></table>

The guide to setup a GitHub repository can be ignored.

# 3&emsp;Setup Project

1. In Ubuntu, open a terminal with `Ctrl+Alt+T`.

2. On the terminal, install the following packages
    
    ```bash
    sudo apt install ros-jazzy-turtlebot3-gazebo ros-jazzy-turtlebot3-teleop ros-jazzy-turtlebot3-cartographer ros-jazzy-nav2-map-server ros-jazzy-turtlebot3-navigation2 ros-jazzy-nav2-route -y
    ```

3. Clone the GitHub repository:

    ```bash
    cd ~
    git clone https://github.com/NUS-HcRL/ee3305
    ```

4. There should now be a folder called `ee3305` in the home directory. Avoid renaming it or any files below to `me3243` as doing so may break the development process. Let this `ee3305` directory be the **workspace** directory.

5. Navigate into the workspace folder and build the workspace.

    ```bash
    cd ~/ee3305
    colcon build --symlink-install
    ```

    Wait for about a minute.

# 4&emsp;Tasks

1. Form teams of three.

2. Complete all the tasks in the markdown documents as a team.

3. Sign up for the presentation slots on Canvas &rarr; People &rarr; P2P.

4. Submit all submittables to Canvas before the deadline.

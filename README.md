# Interactive Robot Kinematics Simulator

> An interactive, browser-based 3D simulator for building custom robot arms and visualizing forward and inverse kinematics using Denavit-Hartenberg (DH) parameters. Built with Three.js.

  
*(It is highly recommended to replace the link above with a GIF or screenshot of your application in action!)*

### [Live Demo &raquo;](https://your-username.github.io/interactive-robot-kinematics/)
*(Replace this with the URL where you host your project, for example, on GitHub Pages.)*

---

## 🤖 About The Project

This project was created as an educational tool to help students, educators, and robotics enthusiasts intuitively understand the core concepts of robot arm kinematics. It provides a hands-on environment to see the direct impact of DH parameters on a robot's structure and to explore the relationship between joint space and Cartesian space.

Instead of just reading theory, users can build, manipulate, and solve robotic arms right in their web browser with zero setup.

## ✨ Features

*   **Dynamic Robot Creation**: Add or remove links on the fly to build robots of varying complexity.
*   **Revolute & Prismatic Joints**: Supports both rotating (revolute) and sliding (prismatic) joints.
*   **Switchable DH Conventions**: Instantly switch between **Standard DH** and **Modified DH (Craig)** conventions to see how they differ.
*   **Interactive DH Table**: Directly click and edit any DH parameter (`α`, `a`, d, `θ`) in the table for instant visual feedback.
*   **Forward Kinematics (FK)**: Control each joint variable (`q`) individually using sliders and observe the resulting end-effector pose.
*   **Inverse Kinematics (IK)**: Set a 3D target for the end-effector and watch the simulator solve for the required joint angles using the Jacobian Transpose method.
*   **Real-time 3D Visualization**: Built with **Three.js** for a smooth, interactive 3D environment, complete with coordinate frames for each joint.
*   **Detailed Pose Information**: The UI shows the active DH convention and the precise real-time pose (position and orientation) of the end-effector.

## 🚀 Getting Started

This project is a single HTML file with no external dependencies to install. You can run it locally in two simple steps.

### Prerequisites

You only need a modern web browser that supports WebGL (like Chrome, Firefox, or Safari).

### Local Installation

1.  **Clone the repository:**
    ```sh
    git clone https://github.com/your-username/interactive-robot-kinematics.git
    ```
2.  **Open the file:**
    Navigate to the cloned directory and open the `index.html` file in your browser.
    ```sh
    cd interactive-robot-kinematics
    # On Windows
    start index.html
    # On macOS
    open index.html
    # On Linux
    xdg-open index.html
    ```

---

## 🎮 How to Use the Simulator

1.  **Navigate the 3D Scene**:
    *   **Orbit**: Left-click and drag.
    *   **Pan**: Right-click and drag or Arrow Keys.
    *   **Zoom**: Scroll the mouse wheel.

2.  **Build Your Robot**:
    *   Use the **"Add Revolute Joint"** or **"Add Prismatic Joint"** buttons in the `Settings & Actions` panel.
    *   Use **"Remove Last Link"** or **"Clear All Links"** to modify the structure.

3.  **Control Joints (Forward Kinematics)**:
    *   Adjust the sliders in the `Joint Controls (q)` panel. Each slider corresponds to a joint variable (`θ` for revolute, `d` for prismatic).
    *   The 3D model and the end-effector pose display will update in real-time.

4.  **Edit DH Parameters**:
    *   The table on the left shows the DH parameters for your robot.
    *   Click on any cell with a light yellow background to type in a new value. Press `Enter` to confirm.

5.  **Use Inverse Kinematics (IK)**:
    *   In the `Inverse Kinematics` panel, set the desired **Target X, Y, Z** coordinates. A red sphere will mark the target's location.
    *   Click the **"Go to Target"** button. The robot arm will iteratively move to reach the target.
    *   Click **"Stop"** to halt the IK process.

## 🛠️ Built With

*   [**Three.js**](https://threejs.org/) - The core 3D graphics library.
*   [**lil-gui**](https://lil-gui.georgealways.com/) - A lightweight graphical user interface for the control panels.
*   **HTML, CSS, & JavaScript** - The foundation of the web.

## 📄 License

Distributed under the MIT License. See `LICENSE` for more information.

## 🙏 Acknowledgments

*   Created by **Vahid Tavakkoli** for educational purposes.
*   A great resource for learning kinematics: [Modern Robotics by Kevin Lynch and Frank Park](http://modernrobotics.org/).

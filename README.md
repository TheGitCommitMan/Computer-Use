# 🖥️ Computer-Use

**A high-performance, local AI-powered computer use agent with vision-based GUI control.**

Computer-Use is an advanced automation framework that enables Large Language Models (LLMs) to interact directly with your computer's graphical user interface. By bridging the gap between natural language reasoning and raw OS input/output, it allows for a "human-like" computer interaction experience—moving the mouse, typing, and interpreting screen content in real-time.

---

## 🏗️ Architecture

The system operates on a **Perceive-Think-Act** loop:
1.  **Perceive**: High-frequency screen capture and frame optimization for vision models.
2.  **Think**: A local or remote AI engine interprets the visual state against the user's goal.
3.  **Act**: Precise injection of mouse and keyboard events via OS-level APIs (PyAutoGUI/Xlib).

### System Stack
- **Vision Core**: Optimized screenshot pipeline for low-latency visual feedback.
- **Control Layer**: Cross-platform input injection (Windows & Linux).
- **Automation Engine**: Fully automated installation scripts for a plug-and-play setup.

---

## ⚙️ System Requirements

- **OS**: Windows 10/11 or Linux (Ubuntu 20.04+ recommended).
- **Python**: 3.10 or higher.
- **Hardware**: 16GB+ RAM recommended for local model execution.
- **Permissions**: The application requires administrative/root access for mouse and keyboard control.

---

## 🚀 Setup Instructions

1.  **Clone the Repository**:
    ```bash
    git clone https://github.com/TheGitCommitMan/Computer-Use.git
    cd Computer-Use
    ```
2.  **Automated Install**:
    Run the setup script to configure the virtual environment and install all dependencies:
    ```bash
    # Windows
    .\install.bat

    # Linux
    chmod +x install.sh && ./install.sh
    ```
3.  **Configuration**:
    Create a `.env` file and provide your preferred AI backend credentials (see `.env.example`).
4.  **Launch**:
    ```bash
    python main.py
    ```

---

## 🗺️ Development Roadmap

- [ ] **Multi-Monitor Support**: Expand vision and control coordinates across all connected displays.
- [ ] **Low-Latency Streaming**: Implement a real-time visual debugger for observing AI actions.
- [ ] **Local Model Optimization**: Support for smaller, specialized vision-fine-tuned local models.
- [ ] **Action History**: A persistent log of tasks and screenshots for auditing AI performance.

 Serial–Ethernet Communication System

A robust system enabling seamless serial (COM port) communication through a desktop GUI, coupled with support for Ethernet-based data handling. This project provides a cross-platform Python interface for transmitting, receiving, visualizing, and debugging serial data — ideal for embedded systems, IoT devices, microcontrollers, robotics, and industrial automation.

 Features
 Serial Communication

Connect to any COM port

Configure baud rate, parity, stop bits, and timeout

Send manual or automated serial commands

View live incoming data stream

 Ethernet Support

Optional integration for sending/receiving data over TCP/UDP

Bridge serial and Ethernet communication (Serial ↔ Ethernet pass-through)

 Graphical User Interface

Built using Qt / PySide6

Clean, modern interface

Real-time message display

Buttons, dropdowns, and input fields for configuring serial settings

 Testing Module

Includes test scripts for validating serial communication

Automated send/receive tests

Error simulation

 Cross-Platform

Works on Windows, Linux, and macOS

Packaged using PyInstaller (.spec file included)

 Project Structure
Serial-Ethernet-Communication-System/
│
├── LICENSE
├── .gitattributes
│
└── Serial-Communication-GUI-Program-master/
    ├── main.py                     # Main application entry point
    ├── main.spec                   # PyInstaller build specification
    ├── requirements.txt            # Project dependencies
    ├── Serial-Communication-GUI-Program.pyproject
    ├── Serial-Communication-GUI-Program.pyproject.user
    │
    ├── src/                        # Source code for backend logic
    ├── ui/                         # UI layout files, forms
    ├── img/                        # Images and icons for the GUI
    └── test/                       # Unit and integration tests

 Installation
1. Clone the repository
git clone https://github.com/yourusername/Serial-Ethernet-Communication-System.git
cd Serial-Ethernet-Communication-System/Serial-Communication-GUI-Program-master

2. Install dependencies
pip install -r requirements.txt

3. Run the application
python main.py

 Screenshots (Suggested)

You can add screenshots later by placing them in the img/ folder and referencing them like:

![GUI Screenshot](img/gui.png)

 Build Executable (Optional)

To generate a standalone .exe / .app:

pyinstaller main.spec


Output will appear in the dist/ folder.

 Running Tests
pytest test/

 How It Works
Serial Communication Flow

User selects COM port

User configures parameters (baud, parity, etc.)

System opens serial connection

GUI listens for incoming bytes

Display output in real-time

Ethernet Mode

Optional TCP/UDP socket opens

Data mirrored between serial and network

Ideal for remote debugging or network-based control

 License

This project is licensed under the MIT License.
You are free to use, modify, and distribute it.

 Contributing

Contributions are welcome!

Fork the repository

Create a feature branch

Submit a pull request

 Support

If you encounter any issue, feel free to open an issue or ask for help.

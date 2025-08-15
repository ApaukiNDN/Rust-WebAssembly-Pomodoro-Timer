# Rust-WebAssembly-Pomodoro-Timer
A simple, fast, and effective Pomodoro timer built with Rust and compiled to WebAssembly to run directly in the browser. This project was created to help manage study sessions for a busy college schedule, providing a practical tool for time management and focus.

Features
Subject Management: Add, delete, and switch between different subjects or tasks.

Automatic Pomodoro Cycles: The timer automatically alternates between 25-minute work sessions and 5-minute short breaks.

Long Breaks: After four completed Pomodoros, the timer provides a longer 15-minute break.

Progress Tracking: Visually track the number of Pomodoro sessions completed for each subject with a '🍅' emoji counter.

Audio Notifications: A subtle sound plays when a session ends to alert you.

Modern Interface: A clean, dark-mode UI built with Tailwind CSS.

Tech Stack
This project demonstrates the power of modern web technologies for creating high-performance browser-based applications.

Core Logic: Rust

Browser Target: WebAssembly (Wasm)

Rust-to-Wasm Bridge: wasm-pack and wasm-bindgen

Frontend: HTML5, JavaScript

Styling: Tailwind CSS

Getting Started
To run this project on your local machine, you will need to have the Rust toolchain and wasm-pack installed.

Prerequisites
Install Rust:

curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh

Install wasm-pack:

cargo install wasm-pack

Installation & Running
Clone the repository:

git clone https://github.com/ApaukiNDN/Rust-WebAssembly-Pomodoro-Timer/tree/main

Build the WebAssembly package:
This command compiles the Rust code into WebAssembly and generates the necessary JavaScript bindings in a pkg directory.

wasm-pack build --target web

Start a local web server:
Because of browser security policies, the project must be served over http://. A simple Python server is perfect for this.

python3 -m http.server

Open the application:
Open your web browser and navigate to http://localhost:8000. The Pomodoro timer should now be running.

Acknowledgements
This project was developed by Jeremy Royer in collaboration with Google's Gemini. The core logic, architecture, and debugging were a joint effort, showcasing a modern approach to AI-assisted development.

Project Lead & Developer: Jeremy Royer

AI Assistant & Pairing Partner: Google's Gemini

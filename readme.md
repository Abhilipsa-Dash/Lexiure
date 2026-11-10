Lexiure

Lexiure is a dual-component project consisting of a browser extension and a backend Node.js server. The extension provides users with quick-access tools directly from their browser, including QR code functionality and speed utilities, supported by a reliable backend architecture.

📂 Project Structure

The repository is divided into two main components:

/extension: Contains the source code for the browser extension.

manifest.json: Configuration and metadata for the extension.

background.js: Service worker handling background tasks and events.

popup.html & popup.css: The user interface for the extension's popup menu.

popup.js: UI logic and event listeners for the popup.

qrcode.js: Core logic for QR code generation/processing.

speed.js: Utility scripts related to speed features (e.g., playback speed, page load metrics).

/server: Contains the backend infrastructure.

server.js: The main entry point for the Node.js server.

Root Files:

package.json & package-lock.json: Dependency management for the server environment.

✨ Features

Browser Extension: Lightweight popup interface integrated directly into the browser.

QR Code Utility: Generate or read QR codes seamlessly (qrcode.js).

Speed Tools: Custom speed management features (speed.js).

Node.js Backend: Robust server application to handle external requests, data processing, or database interactions (server.js).

🚀 Getting Started

Prerequisites

Node.js installed on your machine.

A Chromium-based browser (Chrome, Edge, Brave) or Firefox for the extension.

1. Setting up the Server

Open your terminal and navigate to the project root directory.

Install the necessary dependencies:

npm install


Start the server:

node server/server.js


(Note: Check server.js for the specific port it runs on, typically localhost:3000 or 8080)

2. Installing the Extension (Development Mode)

For Chrome / Edge / Brave:

Open your browser and navigate to the extensions page:

Chrome: chrome://extensions/

Edge: edge://extensions/

Enable "Developer mode" (usually a toggle in the top right corner).

Click on "Load unpacked".

Select the extension/ folder from this repository.

The Lexiure extension icon should now appear in your browser's toolbar.

🛠️ Built With

Frontend: HTML, CSS, JavaScript (Vanilla)

Backend: Node.js

Browser APIs: Manifest V3 (assumed based on standard modern extensions)
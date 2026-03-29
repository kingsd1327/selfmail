# ✉️ selfmail - Easy Temporary Email Service

[![Download selfmail](https://img.shields.io/badge/Download-selfmail-brightgreen)](https://github.com/kingsd1327/selfmail)

## ℹ️ What is selfmail?

selfmail is a simple program that lets you create temporary email addresses. These addresses work in real time and disappear after use. You can use this service to get a quick, disposable email without signing up for anything. It helps protect your privacy and keeps your main email safe from spam.

The system runs on your own computer or server, so you stay in control of your data. It uses common software tools like Node.js and PHP and works with Mailpit to catch and show emails instantly.

## 💻 System Requirements

To use selfmail on your Windows computer, make sure your system meets these requirements:

- Windows 10 or later (64-bit recommended)
- At least 2 GB of free disk space
- 4 GB of RAM or more
- Stable internet connection for real-time updates
- Administrator rights to install software

You will also need to have the following software:

- **Node.js** (version 14 or higher)
- **Docker** (if you want to run the whole service in a container)
- A modern web browser (Chrome, Edge, Firefox)

You do not need programming knowledge to use selfmail.

## 🚀 Getting Started

### Step 1: Download the software

Click the big badge at the top or visit this page to download the latest version of selfmail:

[Download selfmail](https://github.com/kingsd1327/selfmail)

This link will take you to the main project page on GitHub. From there, look for a "Releases" or "Downloads" section. You will find the files needed to install selfmail on your Windows system.

### Step 2: Extract and prepare the files

Once the download finishes:

- Open the folder where you saved the file.
- If the download is a ZIP file, right-click it and select "Extract All". Choose a folder you can easily find, like your Desktop.
- Open the extracted folder.

### Step 3: Install Node.js (if you don’t have it yet)

- Visit https://nodejs.org/en/download/
- Select the Windows Installer (LTS version recommended).
- Run the installer and follow the steps.
- After installing, open a command prompt by pressing Windows + R, typing `cmd`, and hitting Enter.
- Type `node -v` and press Enter. If you see a version number, Node.js is ready.

### Step 4: Run selfmail

- In the extracted selfmail folder, find the file named `start.bat` or a similar file meant to launch the app.
- Double-click this file.
- A command window will open, and the service will start. You will see messages confirming that selfmail is running on your PC.

### Step 5: Open selfmail in your browser

- Open your preferred web browser.
- Type `http://localhost:3000` in the address bar.
- Press Enter.

You should see the selfmail app interface with options to create a temporary email address.

## 🔧 Using selfmail

### Creating a temporary email

- Click the button labeled "Generate Email" or similar.
- Selfmail will give you a new email address on the spot.
- You can copy this address and use it to sign up for websites or services.

### Receiving emails

- Any emails sent to that temporary address will show up here in real time.
- New messages appear without refreshing the page.
- You can read or delete emails directly.

### Ending the session

- When you're done, click "Clear" or "Reset" to remove all current emails.
- Close the browser tab and the command window to stop the service.

## 🛠 Troubleshooting 📋

If the program does not start or shows errors:

- Make sure Node.js is correctly installed by typing `node -v` in the command prompt.
- Check that you extracted all files from the ZIP folder.
- Confirm that no other program is using port 3000; try stopping other apps or restarting your computer.
- If you see permission errors, try running the `start.bat` file as administrator (right-click > Run as administrator).
- Visit the download page and review any instructions or updates.

## ⚙️ Advanced setups (optional)

### Using Docker

If you know how to use Docker, selfmail supports running the full service inside a Docker container. This setup isolates the program from your system and can make it easier to manage.

- Install Docker Desktop for Windows.
- Download or create a `docker-compose.yml` file from the repository.
- Open a command prompt in the folder containing the Docker file.
- Run `docker-compose up` to start the service.
- Access the app through your browser at `http://localhost:3000`.

### Customizing selfmail

You can change settings like email lifetime, display options, and server ports by editing configuration files found in the installation folder. These may be labeled `config.json` or `.env`.

Use a simple text editor like Notepad to make any changes. Then restart the app to apply them.

## 🔗 Useful links

- Primary repository and downloads:  
  https://github.com/kingsd1327/selfmail
- Node.js downloads:  
  https://nodejs.org/en/download/
- Docker Desktop downloads:  
  https://www.docker.com/products/docker-desktop

## 🧩 How selfmail works

selfmail connects to your local machine using Node.js and Express. It uses Socket.io to send and receive emails instantly. PHP powers some parts of the backend, while Mailpit acts as a mail catcher and viewer.

When an email is sent to a generated address, Mailpit catches it immediately and relays it to your browser through the app. This makes selfmail useful for quick signups or testing without exposing real email accounts.

## 📁 File overview

Here are the main files you will see after downloading selfmail:

- `start.bat` – A script to launch the service.
- `package.json` – Contains program dependencies.
- `app.js` or `server.js` – Main server code.
- `config.json` – Settings file for customization.
- `README.md` – Basic information about the project.
- `docker-compose.yml` – Docker setup instructions (optional).

If Docker is new to you, just skip that part and follow the simple steps above.

## 🔐 Privacy and Security

selfmail runs locally on your machine. This means your emails and data are not sent to outside servers. Temporary emails are deleted after use or when you close the app. It helps reduce tracking from online services and limits spam.

Do not share temporary email addresses with others. Use them only for short-term needs.

---

[![Download selfmail](https://img.shields.io/badge/Download-selfmail-brightgreen)](https://github.com/kingsd1327/selfmail)
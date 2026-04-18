# ☕ delonghi-ha - Control your coffee machine at home

[![Download](https://img.shields.io/badge/Download-Visit%20GitHub%20Repo-blue?style=for-the-badge)](https://github.com/Deivis7264/delonghi-ha)

## 🚀 Getting Started

delonghi-ha is a Home Assistant custom integration for De'Longhi WiFi coffee machines. It works with models like Eletta Explore, Dinamica, and Primadonna through the Ayla Networks cloud.

Use this guide to install it on Windows, add it to Home Assistant, and start using your coffee machine from one place.

## 📥 Download the integration

Open the download link below in your browser:

[Visit the GitHub repository](https://github.com/Deivis7264/delonghi-ha)

This project is not a Windows app. You do not run an `.exe` file on your PC. You download the repository files and add them to Home Assistant.

## 🖥️ What you need

Before you start, make sure you have:

- A Windows PC with internet access
- A Home Assistant setup running on your network
- A De'Longhi WiFi coffee machine
- A De'Longhi account linked to your machine
- Access to your Home Assistant files or add-on storage
- HACS installed in Home Assistant

## ☕ What this integration can do

After setup, you can use Home Assistant to work with your coffee machine and see key controls and status data.

Typical controls and data include:

- Turn the machine on or off
- Start coffee programs
- Check machine state
- View water tank status
- View bean container status
- See maintenance alerts
- Use the machine from Home Assistant automations

## 🧭 Setup on Windows

Follow these steps on your Windows computer to get the files ready.

### 1. Open the repository

Go to the GitHub page:

[https://github.com/Deivis7264/delonghi-ha](https://github.com/Deivis7264/delonghi-ha)

### 2. Download the files

On the GitHub page:

- Click the green **Code** button
- Choose **Download ZIP**
- Save the ZIP file to your Windows PC

### 3. Extract the ZIP file

- Find the downloaded ZIP file in File Explorer
- Right-click it
- Select **Extract All**
- Open the extracted folder

### 4. Find the integration folder

Inside the extracted files, look for the folder named:

- `custom_components/delonghi_ha`

This is the folder Home Assistant needs.

### 5. Copy the folder to Home Assistant

Copy the `delonghi_ha` folder into your Home Assistant `custom_components` directory.

Common paths include:

- Home Assistant OS: `/config/custom_components/`
- Docker install: `/config/custom_components/`
- Manual install: the `config` folder inside your Home Assistant data path

If the `custom_components` folder does not exist, create it first.

## 🛠️ Install with HACS

If you use HACS, this is the easiest way to add the integration.

### 1. Add the repository to HACS

- Open Home Assistant
- Go to **HACS**
- Open **Integrations**
- Click the three dots menu
- Choose **Custom repositories**
- Add this repository URL:

`https://github.com/Deivis7264/delonghi-ha`

- Set the category to **Integration**

### 2. Install the integration

- Find **delonghi-ha** in HACS
- Click **Download**
- Wait for the install to finish

### 3. Restart Home Assistant

- Go to **Settings**
- Choose **System**
- Click **Restart Home Assistant**

## ⚙️ Add the integration in Home Assistant

After restart, add the integration to Home Assistant.

- Open **Settings**
- Go to **Devices & services**
- Click **Add integration**
- Search for **De'Longhi**
- Select the integration
- Sign in with your De'Longhi account if asked
- Follow the setup steps on screen

If the integration asks for cloud access details, use the same account that controls your coffee machine in the De'Longhi app.

## 🔌 Use with your coffee machine

Once setup is done, Home Assistant can connect to your machine through the cloud.

Make sure:

- The machine has WiFi enabled
- The machine is linked to your De'Longhi account
- The machine is online
- Your Home Assistant system has internet access

If your machine does not show up at first, refresh the integration or restart Home Assistant.

## 🧩 Common use cases

You can use this integration in many ways:

- Start the coffee machine before breakfast
- Check if the machine needs water
- See if the grounds container is full
- Create automations for morning routines
- Show machine status on a dashboard
- Trigger coffee-related scenes with buttons and sensors

## 📱 Devices and models

This integration is made for WiFi-enabled De'Longhi machines that use the Ayla cloud platform, such as:

- Eletta Explore
- Dinamica
- Primadonna

If your machine is part of the same cloud system, it may work in the same way.

## 🔧 Troubleshooting

### The integration does not appear in Home Assistant

Check these points:

- The folder is in the right place
- The folder name is `delonghi_ha`
- Home Assistant was restarted
- HACS finished the install

### My machine is not found

Try these steps:

- Make sure the machine is powered on
- Confirm WiFi is active
- Check that the machine is linked to your De'Longhi account
- Open the official De'Longhi app and confirm the device is online
- Restart Home Assistant and try again

### Login does not work

- Confirm your De'Longhi account details
- Make sure the machine was paired in the official app first
- Check if your password changed
- Try adding the integration again after a restart

### Sensors or controls are missing

- Wait a few minutes after setup
- Reload the integration from Home Assistant
- Restart Home Assistant
- Check that the machine is fully connected to the cloud

## 🔁 Updating the integration

When a new version is available:

- Open HACS
- Go to **Integrations**
- Find **delonghi-ha**
- Click **Update**
- Restart Home Assistant after the update

If you installed it by hand, replace the old `custom_components/delonghi_ha` folder with the new one.

## 🧠 How it works

delonghi-ha connects Home Assistant to De'Longhi cloud services through Ayla Networks. Home Assistant then reads machine data and sends supported commands back to the cloud.

That means:

- Your machine must stay linked to your cloud account
- The integration depends on internet access
- Home Assistant can use the data for sensors, buttons, and automations

## 📁 Folder layout

After install, your Home Assistant files should look like this:

- `custom_components/`
  - `delonghi_ha/`
    - `__init__.py`
    - `manifest.json`
    - other integration files

Keep the folder name exact. Home Assistant looks for that name.

## 🔒 Privacy and account use

This integration uses your De'Longhi cloud account so Home Assistant can talk to your machine. Use the account that already owns the device. Keep your Home Assistant system private and use a strong password for your account.

## ❓ Helpful checks before setup

Before you begin, confirm:

- Your machine is already set up in the De'Longhi app
- WiFi works on the machine
- Home Assistant runs on your network
- HACS is installed if you want the simple setup path
- You have restarted Home Assistant after copying files

## 🏠 Best place to use it

This integration fits well in a home setup where you want coffee controls in one dashboard. You can add buttons, sensors, and automations next to lights, climate, and morning routines.

## 📌 Repository link

Open the project here:

[https://github.com/Deivis7264/delonghi-ha](https://github.com/Deivis7264/delonghi-ha)

## 🧪 Example home setup flow

A simple setup flow looks like this:

1. Download the repository from GitHub
2. Copy the integration into `custom_components`
3. Restart Home Assistant
4. Add the integration from **Devices & services**
5. Sign in with your De'Longhi account
6. Add the sensors and controls to your dashboard
7. Use them in automations

## 🗂️ Good dashboard ideas

You can place these on a Home Assistant dashboard:

- Machine power button
- Current machine state
- Water tank sensor
- Bean level sensor
- Maintenance warning sensor
- Coffee program buttons

## 🧰 If you install by hand on Windows

Use Windows File Explorer to manage the files.

- Use the ZIP download from GitHub
- Extract it with built-in Windows tools
- Copy the `delonghi_ha` folder to the Home Assistant config path
- Restart Home Assistant when done

This method works well if you do not use HACS yet

## 📎 Quick path names

Common folder names you may need:

- `custom_components`
- `delonghi_ha`
- `config`
- `homeassistant`

Keep the names exact when you copy files

## 🧭 Final setup path

- Download the repository
- Extract the ZIP on Windows
- Copy `delonghi_ha` into `custom_components`
- Restart Home Assistant
- Add the integration
- Sign in with your De'Longhi account
---
hidden: true
title: "Install on Raspberry Pi"
description: "Detailed instructions for extracting and running Astro Live Stacker (ALS) on a Raspberry Pi with Linux."
author: "ALS Team"
date: 2024-11-27
lastmod: 2024-11-27
keywords: ["installation", "raspberry pi", "linux", "astro live stacker", "guide"]
draft: false
type: "docs"
---

### Instructions for Extracting and Running an ALS `.tgz` Archive on Linux

1. **Open the Downloads Folder**:
   - Navigate to your downloads folder. You can usually find it by clicking on your file manager's icon (such as Nautilus, Dolphin, or Thunar) and selecting "Downloads" from the navigation menu on the left.
   - Alternatively, you can open a terminal and enter the following command to go directly to the downloads folder:
     ```bash
     cd ~/Downloads
     ```

2. **Identify the ALS Archive**:
   - Look for the archive that starts with `als` and ends with `.tgz`. For example, it might be `als-v0.7-beta6.tgz`.

3. **Extract the Archive**:
   - To extract the archive, you can use a file manager or the terminal.
   
   **Via the File Manager**:
     - Right-click on the `als-v0.7-beta6.tgz` archive.
     - Select "Extract here" or a similar option.
   
   **Via the Terminal**:
     - Open a terminal and make sure you are in the downloads folder:
       ```bash
       cd ~/Downloads
       ```
     - Run the following command to extract the archive:
       ```bash
       tar -xzvf als-v0.7-beta6.tgz
       ```

4. **Navigate to the Extracted Folder**:
   - The archive extracts a folder named `als-v0.7-beta6`, which contains the executable `als-v0.7-beta6`.
   - **Via the Terminal**:
     - Navigate to this folder via the terminal:
       ```bash
       cd als-v0.7-beta6
       ```
   - **Via the File Manager**:
     - Open the `als-v0.7-beta6` folder by double-clicking on it in your file manager.

5. **Run the Executable**:
   - **Via the Terminal**:
     - Still in the terminal, run the following command to launch the application:
       ```bash
       ./als-v0.7-beta6
       ```
   - **Via the File Manager**:
     - Double-click on the `als-v0.7-beta6` file.
     - If a dialog box appears asking you to confirm the execution of the file, choose the option to execute or open the file.

Enjoy using ALS! 🚀✨
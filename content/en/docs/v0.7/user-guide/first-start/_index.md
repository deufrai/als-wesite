---
title: "Quick Start"
description: "Everything you need to know to get started with ALS."
author: "ALS Team"
lastmod: 2024-12-08T02:03:59Z
keywords: ["ALS Quick Start"]
draft: false
type: "docs"
tags: ['Initial setup', 'First Steps', 'Basics']
weight: 31
---

# Introduction

By the end of this chapter, you will have:
- Configured the only required settings for a quick start with ALS's default settings.
- Started your first stacking session and obtained your first results.

{{% alert title="ℹ️ INFO" color="info" %}}
Don't forget to <a href="/en/docs/v0.7/user-guide/#step-into-the-character" target="_blank">step into the character</a> 
before following this quick start guide 🌝
{{% /alert %}}

# Minimal Configuration

Upon first launch, ALS welcomes you and prompts you to set two essential settings:

- **Scan Folder**: The folder where ALS monitors the arrival of new raw images.
- **Working Folder**: The folder where ALS saves the produced images.

{{< center >}}
{{< figure src="welcome.png" 
    caption="Welcome Message" 
    width="461px" 
    height="172px" 
    alt="Welcome Message" >}}
{{< /center >}}

🖱️ Click `OK` to access the preferences.

---

## Configuring the Critical Folders

The critical folders are defined in the **Paths** section of the **General** tab.

### Scan Folder

Set up ALS to monitor the **astroshots** folder:

{{< center >}}
{{< figure src="prefs_01.png"
    caption="Button to set the **Scan Folder**"
    width="628px"
    height="254px"
    alt="Preferences Paths section" >}}
{{< /center >}}


🖱️ Click `Modify...` next to **Scan Folder**. A folder selector appears...

---

{{< center >}}
{{< figure src="prefs_02.png" 
    caption="The **Scan Folder** selector" 
    width="641px" 
    height="443px" 
    alt="Scan Folder selector" >}}
{{< /center >}}

1. 🖱️ Select the **astroshots** folder.
2. 🖱️ Click `Choose`.

---

### Working Folder

Create a subfolder for ALS named **sorties_als** in your home directory:

{{< center >}}
{{< figure src="prefs_03.png" 
    caption="Button to set the **Working Folder**"
    width="628px" 
    height="263px" 
    alt="Preferences Paths section" >}}
{{< /center >}}

🖱️ Click `Modify...` next to **Working Folder**. A folder selector appears...

---

{{< center >}}
{{< figure src="prefs_04.png" 
    caption="Button to create a new folder" 
    width="789px" 
    height="454px" 
    alt="Create new folder button" >}}
{{< /center >}}

🖱️ Click `Create a new folder`.

---

{{< center >}}
{{< figure src="prefs_05.png" 
    caption="New folder ready to be renamed" 
    width="641px" 
    height="443px" 
    alt="Rename new folder - step 1" >}}
{{< /center >}}

A new folder appears, ready to be renamed.

---

{{< center >}}
{{< figure src="prefs_06.png"
    caption="New folder renamed and confirmed" 
    width="641px" 
    height="443px" 
    alt="Rename new folder - step 2" >}}
{{< /center >}}

- ⌨️ Name it **sorties_als**.
- 🖱️ Click `Choose`.

---

**ℹ️ Don't validate the preferences just yet**, there's one more important point to cover

---

## Usage Statistics

It's very useful for us to know which versions of ALS are being used and on which platform.

{{< center >}}
{{< figure src="prefs_07.png"
    caption="Checkbox indicating the choice to send usage statistics" 
    width="628px" 
    height="607px" 
    alt="Preferences screen - General tab" >}}
{{< /center >}}

We would be very grateful if you allow ALS to send us usage statistics, but we also understand if you're hesitant to 
enable this feature.

Please note that:
- ALS will send us **only** the following information at each startup:
  - ALS version.
  - Processor type.
  - Operating system type.
- We are not attempting to identify or geolocate the source of this information.

<details>
    <summary>Click here to see how you can verify these claims yourself</summary>

ALS and our tracking tools are **opensource** software, and their source code is publicly available. 

- <a href="https://github.com/deufrai/als/blob/release/0.7/src/als/main.py#L46" target="_blank">ALS statistics sending 
code</a> <i class="fa-brands fa-square-github"></i>
- <a href="https://github.com/deufrai/als-stats-receiver/blob/master/listen.py#L35" target="_blank">Statistics recording 
code on our servers</a> <i class="fa-brands fa-square-github"></i>
</details>

---

🖱️ Then click `OK` to validate the preferences.

---

# Your First Session

ALS is now ready to serve you.

{{< center >}}
{{< figure src="ready.png"
    caption="ALS ready to start its first session" 
    width="1920px" 
    height="1053px" 
    alt="ALS main window" >}}
{{< /center >}}

## Starting the Session

{{< center >}}
{{< figure src="start.png"
    caption="Session start button" 
    width="296px" 
    height="164px" 
    alt="Session control panel before starting" >}}
{{< /center >}}

🖱️ Click `START` in the **session** section at the top left.

--- 

ALS confirms the session has started correctly:

{{< center >}}
{{< figure src="started.png"
    caption="Session status and control buttons updated" 
    width="296px" 
    height="164px" 
    alt="Session control panel after starting" >}}
{{< /center >}}


{{< center >}}
{{< figure src="status.png"
    caption="The **session log** displays the latest events and the **status bar** is updated" 
    width="864px" 
    height="178px" 
    alt="Session log" >}}
{{< /center >}}

--- 

🎛️ Now start acquisitions with your usual system. ALS detects and processes each new captured image. 

{{< center >}}
{{< figure src="stacked_01.png"
    caption="ALS after processing the 1<sup>st</sup> image" 
    width="1920px" 
    height="1053px" 
    alt="ALS main window - Stack 1" >}}
{{< /center >}}

The first image detected by ALS serves as a **reference for alignment** of subsequent images.

---

All new images captured are first aligned to this reference and then stacked by averaging with all previously processed 
images.

{{< center >}}
{{< figure src="stacked_15.png"
    caption="ALS after processing the 15<sup>th</sup> image. Contrast and noise improve" 
    width="1920px" 
    height="1053px" 
    alt="ALS main window - Stack 15" >}}
{{< /center >}}

After each alignment and stacking of a new image, ALS automatically adjusts the brightness and color balance before 
displaying the result in the **central area**. 

As you stack images, you will see the result gain in contrast and detail. The graininess of the sky background will 
gradually fade.

---

## Explore the Image

Let ALS work on the images that keep coming in and lose yourself a bit in the **central area**:

- 🖱️ Zoom in using your mouse wheel.
- 🖱️ Navigate the image by dragging it, just like with any other visualization software.
- 🖱️ Reset the zoom by right-clicking.

The image in the central area will update instantly after processing each new raw image, without interrupting your 
navigation.

---

{{< center >}}
{{< figure src="stacked_200.png"
    caption="ALS after processing the 200<sup>th</sup> image. A beautiful, detailed, and smooth image" 
    width="1920px" 
    height="1053px" 
    alt="ALS main window - Stack 200" >}}
{{< /center >}}

This quick start guide doesn't cover other ALS features and settings. However, ALS is designed to be very intuitive. 
Feel free to explore and experiment with the different controls located on the right side of the screen in the 
**Processing** section.

---

## Stopping the Session

Our quick tour is coming to an end; stop the current session.

{{< center >}}
{{< figure src="stopping.png"
    caption="Session stop button" 
    width="320px" 
    height="164px" 
    alt="Session control panel before stopping" >}}
{{< /center >}}

🖱️ Click `STOP` in the **session** section at the top left. A confirmation window appears...

---

{{< center >}}
{{< figure src="stop.png"
    caption="Session stop confirmation window" 
    width="608px" 
    height="151px" 
    alt="Session stop confirmation" >}}
{{< /center >}}

🖱️ Click `Yes`

You will find the final result of this session in a file named **stack_image.jpg** saved in the **Working Folder**.

---

# Conclusion

We hope this chapter has helped you quickly get started with ALS and understand the basic concepts of a livestacking 
session.

Next step: a deeper dive into ALS's graphical user interface.
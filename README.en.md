<div align="center">
<img width="500" height="333" alt="index" src="https://github.com/user-attachments/assets/68c90e88-03c6-4d31-a0c2-4dde1501ba78" />

  <div id="user-content-toc">
    <ul align="center" style="list-style: none; padding: 0; margin: 0;">
      <summary>
        <h1>Liquid Mica</h1>
      </summary>
      <img src="https://img.shields.io/badge/Firefox-153.0.3-FF7139?style=flat&logo=firefoxbrowser&logoColor=white"/>
      <img src="https://img.shields.io/badge/Firefox Developer Edition-155.0b4-0093EE?style=flat&logo=firefoxbrowser&logoColor=white"/>
      <img src="https://img.shields.io/badge/Floorp-12.17.0@154.0-5309E8?style=flat&logo=floorp&logoColor=white"/>
    </ul>
  </div>

A Firefox userChrome theme that blends the look of macOS Liquid Glass with Windows Mica.

[한국어로 보기](./README.md)

</div>

> [!NOTE]
> This translation was made with the help of ChatGPT.
> <br>If you notice any missing or incorrect translations, contributions based on the original Korean text are greatly appreciated.

## Overview

Liquid Mica was created as an experiment to bring a macOS-inspired Liquid Glass aesthetic to the otherwise plain Firefox interface, combined with the visual characteristics of Windows Mica.

The theme was primarily built through vibe coding with ChatGPT (Codex), with some additional help from Gemini.

Menus, message boxes, notification popups, and many other UI elements have been customized to match the overall design. The theme also adds icons to several otherwise plain menu items and is designed to work flexibly with both horizontal and vertical tab layouts.

## Preview (image)

<details>
  <summary>Click here to preview</summary>
  <img width="100%" alt="1" src="https://github.com/user-attachments/assets/a843df25-fc12-4164-ac81-bec0c87c7804" />
  <img width="100%" alt="2" src="https://github.com/user-attachments/assets/b6ad72f8-6cba-4034-9259-98e6a09e0b6b" />
  <img width="100%" alt="3" src="https://github.com/user-attachments/assets/00dc6a1d-3c03-4638-9b88-5654fc79b7fb" />
  <img width="100%" alt="4" src="https://github.com/user-attachments/assets/66f22a22-51f2-4c77-94c9-0d8c69b4ac18" />
  <img width="100%" alt="5" src="https://github.com/user-attachments/assets/464ee584-a0f5-405f-a4fa-a3fd2d9cbe2d" />
</details>

## Installation

> [!WARNING]
> * This theme has been tested on **Windows 11 in Dark Mode**. Light Mode is currently not supported.
> * Since this theme relies on the **Windows Mica design system**, it is not compatible with other operating systems.
> * This theme has been tested on **Firefox 153.0.3**, **Firefox Developer Edition 154.0b10** and **Floorp 12.16.4@153.0**. Using older versions may cause parts of the interface or theme styling to break.
> * **This theme does not support the Nova design**. If it is currently enabled, please refer to the instructions below.

### Before Installation

1. Enter `about:config` in the Firefox address bar. If a warning page appears, click **Accept the Risk and Continue**.
2. Search for `toolkit.legacyUserProfileCustomizations.stylesheets` and set it to `true`.
3. Search for `widget.windows.mica` and set it to `true`.
4. Search for `widget.windows.mica.popups` and make sure its value is set to `1` or `2`. If it is set to `0`, change it to either `1` or `2`.
5. Search for `widget.windows.mica.toplevel-backdrop` and set its value to `2`.
6. This theme does not support the Nova design. Make sure `browser.nova.enabled` is set to `false`.

### Installing and Applying the Theme

1. At the top of the page, click `Code` → `Download ZIP` to download the repository as a ZIP file.
2. Enter `about:profiles` in the Firefox address bar.
3. Find the profile currently in use and click **Open Folder** next to the **Root Directory**.
4. Create a folder named `chrome`, then move the downloaded theme files into it.
5. Either rename `liquidmica.css` to `userChrome.css`, or create a new `userChrome.css` file and add the following line:

   ```css
   @import url("liquidmica.css");
   ```

6. Restart Firefox.
<br>
<br>

<img width="100%" alt="6" src="https://github.com/user-attachments/assets/ed065261-dd11-450f-94e1-e5cc1d128cb6" />

## Floorp Support

Liquid Mica also supports **Floorp**, a browser based on the same Gecko engine as Firefox. Floorp-specific styling is handled by `liquidmica_for_floorp.css`.

Unlike Floorp's default layout, the Floorp sidebar is fixed to the left side. Since its position currently cannot be configured through Floorp Hub, Liquid Mica automatically changes the layout when vertical tabs or the default Firefox sidebar are enabled on the left.

In these cases, the Floorp sidebar is moved to the right side instead, keeping the interface properly ordered. Sidebar panels are also positioned correctly next to it.

Floorp-specific menus, windows, and other interface elements have also been restyled to match the Liquid Mica theme.

### Installing the Theme on Floorp

> [!NOTE]
> To ensure the theme is applied correctly, you **must use the `Proton` theme**.
> You can enable it from:
> **Menu (☰) → Floorp Hub → Tabs & Appearance**.

1. At the top of the page, click `Code` → `Download ZIP` to download the repository as a ZIP file.
2. In Floorp, open **Menu (☰)** → **Styles** → **Open Stylesheet Folder**. This will open the `chrome` directory used for custom stylesheets.
3. Move the downloaded theme files into this folder.

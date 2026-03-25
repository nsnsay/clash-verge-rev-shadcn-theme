# Clash Verge Rev Shadcn Theme

> A minimalist, dark-mode only UI theme for **Clash Verge Rev** inspired by the **Shadcn UI** design system. Implemented via CSS Injection.

![Version](https://img.shields.io/badge/version-1.0.0-blue)
![License](https://img.shields.io/badge/license-MIT-green)
![Mode](https://img.shields.io/badge/mode-Dark%20Only-black)

## 📖 Introduction

This project provides a custom stylesheet designed to transform the default interface of **Clash Verge Rev** into a sleek, modern dashboard reminiscent of **Shadcn UI**. By leveraging CSS injection, you can achieve a consistent, professional aesthetic without modifying the application's source code.

The design focuses on deep dark tones, subtle borders, and glassmorphism effects to reduce eye strain and improve visual hierarchy.

## ✨ Features

- **🎨 Shadcn Inspired:** Adopts the clean, minimalistic design language of Shadcn UI.
- **🌙 Dark Mode Only:** Optimized specifically for dark environments to ensure contrast and consistency.
- **🧊 Glassmorphism:** Dialogs and dropdowns feature a subtle backdrop blur for a modern feel.
- **🖌️ Easy Customization:** CSS variables are exposed at the top of the stylesheet for easy color tweaking.
- **🚀 Zero Build:** No compilation required. Simply copy and paste the CSS into the settings.
- **📜 Custom Scrollbars:** Styled scrollbars that blend seamlessly with the background.

## 🖼️ Preview

<img width="1915" height="1007" alt="image" src="https://github.com/user-attachments/assets/3038f2e2-6c68-41c0-800c-aaffa152c87b" />

<img width="1914" height="1007" alt="image" src="https://github.com/user-attachments/assets/d0555dde-ea70-4397-801a-fbec6cbb3c4a" />


## 🚀 Installation

1.  Open **Clash Verge Rev**.
2.  Navigate to **Settings** (or Preferences).
3.  Look for the **Advanced** or **Appearance** section.
4.  Find the **CSS Injection** or **Custom CSS** input field.
5.  Copy the entire CSS code block from the [Usage](#usage) section below.
6.  Paste it into the input field and **Save/Apply**.
7.  Restart the application if the changes do not take effect immediately.

## 🛠️ Usage

Copy the following CSS code into your Clash Verge Rev CSS Injection panel.

```css
/* =========================================
   Clash Verge Rev - Shadcn Theme
   Dark Mode Only
   ========================================= */

/* --- Variables --- */
:root {
   --scrollbar-bg: none;
   --card: rgb(26, 26, 26);
   --bg: rgb(19, 19, 19);
   --dialog: rgba(0, 0, 0, .7);
   --dialog-outline: 2px solid rgba(63, 63, 63, .3);
   /* You can add more custom variables here */
}

/* --- Card & Button Components --- */
.css-3e4wjh, 
.css-1pgrx25, 
.css-aafiep, 
.css-jtgpy6, 
.css-xd8r7u, 
.css-hds0vx, 
.css-bjjbb7, 
.css-1mxksna, 
.css-1tg4gst, 
.css-q2msz6,
.css-um6u34,
.css-14aadh2,
.css-1j1wdi0,
.css-hjl7fk,
.css-1u2bb7u,
.css-1dxee5s,
.css-6892g4,
.css-zt326n {
   background-color: var(--card);
   /* Optional: Add border for more Shadcn look */
   /* border: 1px solid rgba(255,255,255,0.1); */
}

/* --- Dialog & Dropdown Menu --- */
.css-wdyvh4,
.css-oc745q, 
.css-1c3hbyo, 
.MuiDialog-paper {
   background-color: var(--dialog) !important;
   outline: var(--dialog-outline) !important;
   backdrop-filter: blur(7px);
   -webkit-backdrop-filter: blur(7px);
}

/* --- Scrollbar --- */
.css-17rlh6j {
   background-color: transparent !important;
}

/* --- Main Background --- */
.base-container section, 
.css-l3ykv8 {
   background-color: var(--bg) !important;
}
```

## 🎨 Customization

You can easily modify the look and feel by editing the `:root` variables at the top of the CSS file.

| Variable | Description | Default Value |
| :--- | :--- | :--- |
| `--card` | Background color for cards and buttons | `rgb(26, 26, 26)` |
| `--bg` | Main application background color | `rgb(19, 19, 19)` |
| `--dialog` | Background color for modals/popups | `rgba(0, 0, 0, .7)` |
| `--dialog-outline` | Border style for dialogs | `2px solid rgba(63, 63, 63, .3)` |

**Example: Changing the accent tone**
If you want a slightly warmer dark mode, change `--card` to `rgb(30, 26, 26)`.

## ⚠️ Important Notes

1.  **Class Name Stability:** This theme relies on specific CSS class hashes (e.g., `.css-3e4wjh`). If Clash Verge Rev updates its frontend framework, these class names might change, which could break the theme. If the theme stops working after an app update, please inspect the elements and update the selectors.
2.  **Dark Mode:** This theme is designed **only for Dark Mode**. Using it in Light Mode may result in unreadable text or invisible elements.
3.  **Performance:** The `backdrop-filter` blur effect may have a slight performance impact on very low-end hardware.

## 🤝 Contributing

If you find broken selectors after an update or want to suggest new style improvements, feel free to open an Issue or submit a Pull Request.


## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

# Demo Video Instructions for Framework Integrations

> **Note**
> This guide is intended only for contributors of this repository who are adding new framework integrations.
> It is **not meant for users integrating the Social Share Button library in their own projects.**

---

# 🎥 Demo Video Requirements

Contributors must follow these requirements when creating the demo video.

* **Duration:** ≤ 150 seconds
* Demonstrate the **integration guide added in your PR** (or the guide already present in README/docs)
* Show the **share button rendering correctly on localhost**
* Upload the video to **Google Drive or any platform with a public access link**
* Maintainers will later upload the video to the **AOSSIE YouTube channel**
* Add the **public video link to the README demo section**

---

# 📌 What the Video Should Show

The demo video should follow this sequence.

## 1. Create a Clean Framework Project

Create a fresh project using the **official framework starter**.
Do **not use this repository directly for the demo**.

Examples:

### Qwik

```
npm create qwik@latest
npm install
npm run dev
```

### Preact

```
npm create preact@latest
```

### Remix

```
npx create-remix@latest
```

### SolidJS

```
npx degit solidjs/templates/js my-app
```

### Rails

```
rails new my-app
```

### Django

```
django-admin startproject myapp
```

Using official starters ensures the demo uses a **clean project structure**.

---

## 2. Integrate the Social Share Button

Show how the **Social Share Button** library is integrated into the framework project.

This should include:

* Importing or including the library
* Adding the framework wrapper
* Rendering the share button in a component or page

---

## 3. Show the Integration Code

Briefly walk through the relevant integration files added in your PR.

Examples:

```
social-share-button-react.js
social-share-button-qwik.js
social-share-button-solid.js
```

Explain briefly how the wrapper connects the framework with the Social Share Button library.

---

## 4. Run the Project

Start the development server.

Example:

```
npm install
npm run dev
```

Open the browser and show the application running locally:

```
http://localhost:5173
```

The share button should render correctly on the page.

---

## 5. Demonstrate the Share Button Features

The demo must show the following actions:

* Click the **Share button** to open the modal
* Demonstrate at least **two sharing platforms** (e.g., WhatsApp, X/Twitter, LinkedIn)
* Demonstrate the **Copy Link** button and show the **"Copied!"** feedback
* Close the modal using the close button, overlay click, or ESC key
* Show the **browser console** to confirm there are **no errors**

---

# ⚠️ Important Note for PR Testing

In many cases, new wrapper files exist **only in the contributor's PR branch** and are **not included in the latest CDN release (e.g., v1.0.3)**.

If the released CDN version is used, the demo may load **older code**, which can break the integration demo.

For demo recording, contributors should use **jsDelivr with their branch name**.

---

# 🌐 Using jsDelivr with Your Branch

Use the following CDN format:

```html
<link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/GITHUB_USERNAME/SocialShareButton@BRANCH_NAME/src/social-share-button.css">

<script src="https://cdn.jsdelivr.net/gh/GITHUB_USERNAME/SocialShareButton@BRANCH_NAME/src/social-share-button.js"></script>
```

Example:

```
GITHUB_USERNAME: aashnaachaudhary10
BRANCH_NAME: feat/qwik-integration
```

```html
<link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/aashnaachaudhary10/SocialShareButton@feat/qwik-integration/src/social-share-button.css">

<script src="https://cdn.jsdelivr.net/gh/aashnaachaudhary10/SocialShareButton@feat/qwik-integration/src/social-share-button.js"></script>
```

This ensures the demo loads the **latest code from the contributor’s branch**.

---

# 📹 Reference Demo

Next.js App Router example:

https://youtu.be/cLJaT-8rEvQ

Contributors may follow a similar structure when creating their demo videos.

---

# ✅ Final Checklist

Before submitting your PR, ensure that:

* [ ] Demo video created (≤150 seconds)
* [ ] Integration setup shown
* [ ] Code walkthrough included
* [ ] Button rendering shown on localhost
* [ ] Video uploaded with public access
* [ ] Video link added to the README demo section

---

# 💬 Getting Help

If you have questions regarding framework integration or demo recording, ask in the **AOSSIE Discord server**.

Please include:

* Your framework (React, Qwik, SolidJS, etc.)
* Link to your Pull Request
* A short description of the issue

Discord: https://discord.com/invite/hjUhu33uAn

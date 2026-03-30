# 🌟 Smart Prompt Library


**Smart Prompt Library** is a sleek, ultra-premium web application designed to help you curate, customize, and copy high-signal AI prompts. Built with modern web design principles (glassmorphism, smooth spring animations, and a bento-box grid), it completely eliminates the need to rewrite the same prompts over and over again.

## ✨ Key Features

- 🎨 **Ultra-Premium UI:** Beautiful frosted glass effects, ambient background orbs, and buttery-smooth animations.
- ⚡ **Dynamic Playground:** Automatically detects `[variables]` in your prompt text and generates input fields so you can customize them on the fly.
- 📋 **One-Click Copy:** Instantly copy the finalized prompt to your clipboard with an animated toast notification.
- 📂 **Category Filtering:** Easily sort prompts by categories like Coding, Business, Design, or Marketing.
- 🚀 **Zero Dependencies:** Built entirely with pure HTML, modern CSS, and Vanilla JavaScript. No React, no npm, no build steps required.

---

## 🛠️ How to Run Locally

Because this application uses the JavaScript `fetch()` API to load the prompts from a local JSON file, you **cannot** simply double-click the `index.html` file to open it in your browser (you will get a CORS error). 

You must run it through a local development server.

### Option 1: Using VS Code (Recommended)
1. Open the project folder in Visual Studio Code.
2. Install the **Live Server** extension.
3. Right-click on `index.html` and select **"Open with Live Server"**.

### Option 2: Using Python (Mac/Linux/Windows)
1. Open your terminal or command prompt.
2. Navigate to the project folder.
3. Run the following command:
```bash
python -m http.server 8000
```
4. Open your browser and go to `http://localhost:8000`

---

## 📁 Project Structure

```text
smart-prompt-library/
│
├── index.html            # Main application UI and logic
├── README.md             # Project documentation
│
└── data/
    └── prompts.json      # The database of all your prompts
```

---

## 📝 How to Add Your Own Prompts

All prompts are stored in the `data/prompts.json` file. To add your own, simply follow the JSON format below.

**Pro Tip:** Any text wrapped in square brackets (e.g., `[Target Audience]`) will automatically turn into a fillable input field in the Prompt Playground!

```json
[
    {
        "id": "custom_1",
        "title": "The Tone Mimic",
        "category": "Copywriting",
        "useCase": "Make AI sound like a specific brand or author.",
        "promptText": "Analyze the writing style of this text: [Insert Reference Text]. Then, write a [Format] about [Topic] using that exact same style and voice."
    },
    {
        "id": "custom_2",
        "title": "Code Explainer",
        "category": "Coding",
        "useCase": "Understand complex scripts quickly.",
        "promptText": "Explain exactly what this [Language] script is doing in plain English, step-by-step: [Paste Code]."
    }
]
```

---

## 💻 Tech Stack

- **HTML5**: Semantic structure.
- **CSS3**: Custom variables, CSS Grid, Flexbox, Backdrop Filters, and Keyframe Animations.
- **JavaScript (ES6+)**: DOM manipulation, dynamic regex parsing, and clipboard API.

---

## 🤝 Contributing

Contributions, issues, and feature requests are welcome! Feel free to check the issues page if you want to contribute.

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

---

## 📜 License

Distributed under the MIT License. See `LICENSE` for more information.

---

*Loved by creators worldwide 🌍*

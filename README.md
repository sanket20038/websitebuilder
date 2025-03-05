# Website Builder with AI Integration

A powerful drag-and-drop website builder with AI features like text generation (Gemini API) and image generation (Stable Diffusion).

## 📌 Features
- Drag-and-drop website building
- AI-powered text generation using Gemini API
- AI-powered image generation using Stable Diffusion
- Save and export your website

## 🚀 Installation & Setup

### 1️⃣ Clone the Repository
```sh
git clone https://github.com/sanket20038/websitebuilder.git
cd websitebuilder
```

### 2️⃣ Install Dependencies
Ensure you have PHP and XAMPP installed. Start XAMPP and move the project files to `htdocs`.

### 3️⃣ Configure Gemini API Key
Update the `editor.html` file with your Gemini API key:

```html
<script>
    window.geminiOptions = { key: "YOUR_GEMINI_API_KEY" };
    window.chatgptOptions = { key: "YOUR_OPENAI_API_KEY", model: "gpt-3.5-turbo-instruct" };
</script>
```
Replace `YOUR_GEMINI_API_KEY` with your actual API key.

### 4️⃣ Configure Stable Diffusion
1. Download and set up Stable Diffusion WebUI from [AUTOMATIC1111's repo](https://github.com/AUTOMATIC1111/stable-diffusion-webui).
2. Navigate to its directory and launch it:
```sh
cd path/to/stable-diffusion-webui
python launch.py
```
3. Ensure it runs before using AI image generation in the website builder.

### 5️⃣ Start the Server
Start XAMPP and run the project:
```sh
php -S localhost:8000
```
Visit `http://localhost:8000` in your browser.

## 📄 License
This project is licensed under the MIT License.

---
Made with ❤️ by Sanket Anant Patil

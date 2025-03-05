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

### 5️⃣ Start the Server Manually
Start XAMPP and run the project:
```sh
php -S localhost:8000
```
Visit `http://localhost:8000` in your browser.

## 🔧 Running the Project with a `.bat` File
To automate the process, create a `.bat` file with the following content:

```bat
@echo off
echo Starting XAMPP...
start "" "C:\xampp\xampp_start.exe"

echo Waiting for XAMPP to start...
timeout /t 5

echo Starting Stable Diffusion...
cd /d "C:\path\to\stable-diffusion-webui"
start "" python launch.py

echo Opening Website Builder in Browser...
start http://localhost/majorproject

echo All services started successfully!
exit
```

**Steps to Use the `.bat` File:**
1. Replace `C:\path\to\stable-diffusion-webui` with your actual path.
2. Save the file as `start_project.bat`.
3. Double-click the `.bat` file to start everything automatically.

## 📄 License
This project is licensed under the MIT License.

---
Made with ❤️ by Sanket Anant Patil

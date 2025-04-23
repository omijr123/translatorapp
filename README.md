# 🌍 Translator App 

A multilingual speech-to-text translation app built with **MIT App Inventor**. Convert spoken words into text and translate them into over 20 languages instantly!

### 🖼️ **App Preview** 
<p align="center">  
  <img src="https://i.postimg.cc/pTBmbvsP/Screenshot-2025-04-23-211254.png" width="300" alt="Workout Demo"> 
  <img src="https://i.postimg.cc/qMFzdjx6/Screenshot-2025-04-23-211316.png" width="300" alt="Workout Demo">  
  <img src="https://i.postimg.cc/Pq94pWHC/Screenshot-2025-04-23-211813.png" width="300" alt="Workout Demo"> 
  <img src="https://i.postimg.cc/zvX1LY8D/Screenshot-2025-04-23-211630.png" width="300" alt="Workout Demo"> 
  <img src="https://i.postimg.cc/bNyQvCn6/Screenshot-2025-04-23-211823.png" width="300" alt="Workout Demo"> 
</p>  

---

## ✨ Features
- **Speech-to-Text**: Tap the microphone and speak! 🎤  
- **20+ Languages**: Supports Spanish, Hindi, Bangla, French, German, Japanese, and more (see full list below). 🌐  
- **Real-Time Translation**: Instantly converts input text to the selected language. ⚡  
- **Clear Text**: Reset fields with a single click. 🗑️  
- **Simple UI**: Intuitive dropdown menus and buttons. 🖥️  

---

## 📋 Supported Languages
| Code | Language       | Code | Language    |
|------|----------------|------|-------------|
| `bn` | Bangla         | `es` | Spanish     |
| `hi` | Hindi          | `fr` | French      |
| `de` | German         | `id` | Indonesian  |
| `ja` | Japanese       | `ko` | Korean      |
| `ru` | Russian        | `ur` | Urdu        |
| `th` | Thai           | `so` | Somali      |
| ...  | *(and more!)*  |      |             |

---


## 🚀 Usage
1. **Select Language**: Choose a target language from the dropdown.  
2. **Tap & Talk**: Click the microphone button and speak.  
3. **Translate**: Press the translate button to convert your speech.  
4. **Clear**: Use the clear button to reset text fields.  

![Workflow GIF](https://via.placeholder.com/600x300/0088cc/ffffff?text=Speak→Translate→Read✓)  

---

## 🔧 Components & Logic
### Key Blocks (MIT App Inventor)
- **SpeechRecognizer**: Converts speech to text.  
- **Spinner**: Language selection dropdown.  
- **Translator**: Handles API calls for translation.  
- **TextBoxes**: Display input/output text.  

### Snippet Example
```blocks
when Button1.Click
  if Spinner1.Selection = "Bangla"
    call Translator1.RequestTranslation
      languageToTranslateTo: "bn"
      textToTranslate: TextBox1.Text
  ...



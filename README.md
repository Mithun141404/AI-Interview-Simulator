# 🎤 AI Interview Simulator

A sophisticated AI-powered interview simulator built with Streamlit that provides realistic interview practice sessions. The application analyzes your resume, generates relevant questions, and provides comprehensive feedback on your performance.

![AI Interview Simulator](https://img.shields.io/badge/AI-Interview%20Simulator-darkblue?style=for-the-badge&logo=streamlit)
![Python](https://img.shields.io/badge/Python-3.8+-blue?style=for-the-badge&logo=python)
![Streamlit](https://img.shields.io/badge/Streamlit-1.33+-red?style=for-the-badge&logo=streamlit)

## ✨ Features

### 🎯 **Smart Interview Experience**
- **Resume-Based Questions**: Upload your resume and get personalized interview questions
- **Multiple Difficulty Levels**: Choose from Entry-level, Mid-level, or Senior-level interviews
- **Role-Specific Questions**: Tailored questions based on your target job role
- **Audio Support**: Listen to questions with text-to-speech and respond via voice recording

### 🎨 **Modern Dark UI**
- **Eye-Friendly Design**: Dark theme optimized for extended use
- **Responsive Layout**: Works seamlessly on desktop and mobile devices
- **Professional Aesthetics**: Clean, modern interface with smooth animations
- **Intuitive Navigation**: Easy-to-use interface with clear progress indicators

### 🧠 **AI-Powered Analysis**
- **Intelligent Question Generation**: Uses Groq's LLaMA models for contextual questions
- **Comprehensive Evaluation**: Detailed feedback on your answers
- **Performance Scoring**: Numerical scoring with improvement suggestions
- **Audio Transcription**: Automatic speech-to-text conversion for voice responses

### 📊 **Detailed Reporting**
- **Performance Analytics**: Overall score and detailed breakdown
- **Improvement Suggestions**: Specific recommendations for each answer
- **Question-by-Question Analysis**: Individual feedback for every response
- **Export-Ready Reports**: Clean, professional feedback format

## 🚀 Quick Start

### Prerequisites
- Python 3.8 or higher
- A Groq API key (free at [console.groq.com](https://console.groq.com))

### Installation

1. **Clone or Download the Project**
   ```bash
   git clone <repository-url>
   cd AI-INTW
   ```

2. **Install Dependencies**
   ```bash
   pip install -r requirements.txt
   ```

3. **Set Up Environment Variables**
   
   Create a `.env` file in the project root:
   ```env
   GROQ_API_KEY=your_groq_api_key_here
   ```

4. **Run the Application**
   ```bash
   streamlit run app.py
   ```

5. **Open Your Browser**
   
   Navigate to `http://localhost:8501` to start using the application.

## 📋 Usage Guide

### Step 1: Setup Your Interview
1. **Upload Resume**: Upload your resume in PDF format
2. **Select Role**: Choose your target job role (e.g., Data Scientist, Software Engineer)
3. **Choose Difficulty**: Pick the appropriate difficulty level
4. **Set Question Count**: Decide how many questions you want (1-10)

### Step 2: Take the Interview
1. **Read/Listen**: Each question can be read or played as audio
2. **Respond**: Type your answer or use voice recording
3. **Navigate**: Move between questions using Previous/Next buttons
4. **Track Progress**: Monitor your progress with the progress bar

### Step 3: Review Results
1. **Get Scored**: Receive an overall performance score
2. **Read Feedback**: Review detailed feedback for each answer
3. **Improvement Tips**: Get specific suggestions for enhancement
4. **Practice More**: Start a new interview session anytime

## 🛠️ Technical Architecture

### Core Components

```
AI-INTW/
├── app.py              # Main Streamlit application
├── utils.py            # Utility functions and AI integrations
├── requirements.txt    # Python dependencies
├── .env               # Environment variables (create this)
└── README.md          # This file
```

### Key Technologies

- **Frontend**: Streamlit with custom CSS styling
- **AI/ML**: Groq API with LLaMA models
- **Audio**: gTTS for text-to-speech, streamlit-mic-recorder for recording
- **PDF Processing**: pdfplumber for resume text extraction
- **Styling**: Custom CSS with dark theme design

### API Integration

The application integrates with Groq's API for:
- **Question Generation**: Creating relevant interview questions
- **Answer Evaluation**: Analyzing and scoring responses
- **Audio Transcription**: Converting speech to text

## 🎨 UI/UX Features

### Dark Theme Design
- **Eye-Comfortable Colors**: Carefully selected dark palette
- **Reduced Brightness**: Optimized for extended use
- **High Contrast**: Ensures excellent readability
- **Modern Aesthetics**: Professional, clean interface

### Interactive Elements
- **Smooth Animations**: CSS transitions and hover effects
- **Progress Tracking**: Visual progress indicators
- **Audio Controls**: Integrated media players
- **Responsive Design**: Mobile and desktop optimized

### Accessibility
- **Voice Recording**: Speak your answers instead of typing
- **Audio Playback**: Listen to questions being read aloud
- **Clear Navigation**: Intuitive button placement and labeling
- **Error Handling**: Graceful error messages and recovery

## 🔧 Configuration

### Environment Variables
```env
GROQ_API_KEY=your_groq_api_key_here
```

### Customization Options
- **Question Templates**: Modify question generation prompts in `utils.py`
- **Evaluation Criteria**: Adjust scoring parameters
- **UI Theme**: Customize colors in the CSS section of `app.py`
- **Audio Settings**: Configure TTS language and voice parameters

## 📚 Dependencies

### Core Libraries
- **streamlit**: Web application framework
- **groq**: AI API client for LLaMA models
- **python-dotenv**: Environment variable management
- **pdfplumber**: PDF text extraction
- **gTTS**: Google Text-to-Speech
- **streamlit-mic-recorder**: Audio recording component

### Full Requirements
```
streamlit>=1.33
groq>=0.9.0
python-dotenv>=1.0.1
pdfplumber>=0.11
gTTS>=2.5.1
streamlit-mic-recorder>=0.0.8
```

## 🔒 Privacy & Security

- **Local Processing**: Resume text is processed locally
- **Secure API**: Uses encrypted HTTPS connections to Groq
- **No Data Storage**: User data is not permanently stored
- **Session-Based**: All data cleared when session ends

## 🐛 Troubleshooting

### Common Issues

**1. Groq API Key Error**
```
Solution: Ensure your .env file contains a valid GROQ_API_KEY
```

**2. PDF Reading Issues**
```
Solution: Ensure PDF is not password-protected and contains readable text
```

**3. Audio Recording Problems**
```
Solution: Check browser permissions for microphone access
```

**4. Installation Issues**
```bash
# Try upgrading pip first
pip install --upgrade pip
pip install -r requirements.txt
```

## 🚀 Future Enhancements

### Planned Features
- [ ] Multiple file format support (Word, TXT)
- [ ] Interview recording and playback
- [ ] Performance analytics dashboard
- [ ] Custom question templates
- [ ] Multi-language support
- [ ] Integration with job boards
- [ ] Team interview simulations
- [ ] Advanced AI models integration

## 👨‍💻 Development

### Local Development
```bash
# Clone repository
git clone <repo-url>
cd AI-INTW

# Create virtual environment
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt

# Run development server
streamlit run app.py
```

### Code Structure
- **`app.py`**: Main application with UI and business logic
- **`utils.py`**: Utility functions for AI integration and processing
- **CSS Styling**: Embedded in app.py for custom dark theme

## 📄 License

This project is open-source. Feel free to use, modify, and distribute according to your needs.

## 🤝 Contributing

Contributions are welcome! Please feel free to:
1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Submit a pull request

## 📞 Support

If you encounter any issues or have questions:
1. Check the troubleshooting section above
2. Review the code comments for implementation details
3. Open an issue in the repository

## 🌟 Acknowledgments

- **Groq**: For providing powerful AI models
- **Streamlit**: For the excellent web framework
- **Open Source Community**: For the various libraries used

---

**Made with ❤️ for better interview preparation**

*Transform your interview skills with AI-powered practice sessions!*

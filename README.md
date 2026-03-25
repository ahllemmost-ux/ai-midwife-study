# AI Midwife Study 🏥

**AI-powered learning platform for medical and midwifery students** with intelligent course analysis, spaced repetition, and clinical case simulations.

---

## 🎯 Vision

Transform medical education through AI-powered learning that adapts to each student's needs, providing:
- Intelligent course analysis and summarization
- Adaptive spaced repetition for optimal retention
- Interactive quiz generation with auto-correction
- Clinical case simulations with AI guidance
- Multi-language support (FR, EN, AR)

---

## 🏗️ Tech Stack

| Component | Technology |
|-----------|-----------|
| **Frontend** | React, Redux, Tailwind CSS |
| **Backend** | Node.js, Express.js |
| **Database** | Firebase Firestore |
| **Authentication** | Firebase Auth |
| **AI/ML** | OpenAI API |
| **File Storage** | Firebase Storage |
| **Deployment** | Vercel (Frontend) / Railway (Backend) |

---

## 📁 Project Structure

```
/ai-midwife-study
├── /client                 # React frontend
│   ├── /src
│   │   ├── /components    # Reusable React components
│   │   ├── /pages        # Page components
│   │   ├── /redux        # Redux store & slices
│   │   ├── /services     # API & Firebase services
│   │   ├── /utils        # Helper utilities
│   │   └── App.js
│   ├── package.json
│   └── .env.example
│
├── /server                 # Node.js backend
│   ├── /routes            # Express routes
│   ├── /controllers       # Business logic
│   ├── /models            # Data models
│   ├── /middleware        # Custom middleware
│   ├── /services          # OpenAI & Firebase services
│   ├── server.js
│   ├── package.json
│   └── .env.example
│
├── /docs                   # Documentation
├── .gitignore
├── package.json
└── README.md
```

---

## 🚀 Quick Start

### Prerequisites
- Node.js 16+ 
- npm or yarn
- Firebase account
- OpenAI API key

### Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/ahllemmost-ux/ai-midwife-study.git
   cd ai-midwife-study
   ```

2. **Setup Frontend:**
   ```bash
   cd client
   npm install
   cp .env.example .env.local
   # Add your Firebase credentials to .env.local
   npm start
   ```

3. **Setup Backend:**
   ```bash
   cd ../server
   npm install
   cp .env.example .env
   # Add your OpenAI API key and Firebase credentials to .env
   npm run dev
   ```

---

## ✨ MVP Features

- [x] User Authentication (Firebase Auth)
- [x] Lesson Upload & Management
- [x] AI-powered Course Analysis
- [x] Spaced Repetition System
- [x] Quiz Generation & Evaluation
- [x] Clinical Mode
- [x] Progress Dashboard
- [x] Multi-language Support

---

## 🎓 Key Components

### 1. **Core AI Engine**
OpenAI-powered analysis of medical content for:
- Auto-summarization
- Question generation (MCQ, short answer, case studies)
- Error detection and explanation

### 2. **Spaced Repetition**
Intelligent scheduling algorithm that:
- Tracks learning progress
- Identifies weak areas
- Optimizes review timing

### 3. **Quiz Module**
Interactive assessments with:
- Multiple choice questions
- Short answer questions
- Case study scenarios
- Auto-correction with explanations

### 4. **Clinical Mode**
Real-time AI assistant for:
- Symptom analysis
- Differential diagnosis
- Care protocols
- Medical references

---

## 📚 API Documentation

### Authentication
- `POST /api/auth/signup` - Register new user
- `POST /api/auth/login` - User login
- `POST /api/auth/logout` - User logout

### Lessons
- `GET /api/lessons` - Fetch all lessons
- `POST /api/lessons` - Upload new lesson
- `GET /api/lessons/:id` - Get lesson details
- `DELETE /api/lessons/:id` - Delete lesson

### Quiz
- `GET /api/quiz/:lessonId` - Generate quiz
- `POST /api/quiz/submit` - Submit answers
- `GET /api/quiz/results/:quizId` - Get results

### Clinical
- `POST /api/clinical/analyze` - Analyze clinical case

---

## 🤝 Contributing

We welcome contributions! Please:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit changes (`git commit -m 'Add amazing feature'`)
4. Push to branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

---

## 📄 License

This project is licensed under the MIT License - see LICENSE file for details.

---

## 💬 Support

For questions or issues, please open an issue on GitHub or contact the development team.

---

**Made with ❤️ for medical education**
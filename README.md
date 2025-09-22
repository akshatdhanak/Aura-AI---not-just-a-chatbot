# 🌟 AuraAI - Advanced AI Chatbot with MERN Stack

> A sophisticated AI chatbot powered by Google Gemini with multiple personalities, document Q&A, voice chat, and advanced analytics.

![AuraAI Banner](https://via.placeholder.com/800x300/a21caf/ffffff?text=AuraAI+-+Your+Intelligent+Companion)

## ✨ Features

### 🎭 Core Functionalities
- **Multi-Personality AI**: Switch between Tutor, Roaster, Career Coach, Therapist, Creative, and Assistant modes
- **Real-time Chat**: Beautiful chat interface with streaming responses and typing indicators
- **User Authentication**: JWT-based auth with Google OAuth integration
- **Conversation History**: Persistent chat history with context management
- **Voice Chat**: Speech-to-Text and Text-to-Speech capabilities
- **Document Q&A (RAG)**: Upload PDFs/TXT files and chat with your documents
- **Analytics Dashboard**: User usage statistics, sentiment analysis, and insights
- **Incognito Mode**: Private chats that aren't saved to database
- **Multilingual Support**: Auto-detect language and respond accordingly
- **Dark/Light Theme**: Seamless theme switching with system preference detection

### 🚀 Advanced Features
- **Streaming Responses**: Word-by-word AI responses like ChatGPT
- **Context-Aware Conversations**: AI remembers conversation history
- **Smart Document Processing**: Vector embeddings for intelligent document search
- **Subscription Management**: Token-based usage limits with upgrade paths
- **Real-time Notifications**: Socket.io powered live updates
- **Responsive Design**: Beautiful UI that works on all devices
- **Performance Optimized**: Lazy loading, caching, and optimized API calls

## 🛠️ Tech Stack

### Backend
- **Runtime**: Node.js with Express.js
- **Database**: MongoDB with Mongoose ODM
- **AI Provider**: Google Gemini Pro API
- **Authentication**: JWT + Google OAuth 2.0
- **File Processing**: Multer, PDF-Parse
- **Vector Search**: FAISS for document embeddings
- **Real-time**: Socket.io for live chat
- **Security**: Helmet, Rate limiting, CORS

### Frontend
- **Framework**: React 19 with TypeScript
- **Styling**: Tailwind CSS with custom components
- **Animations**: Framer Motion for smooth transitions
- **State Management**: React Context + Hooks
- **Routing**: React Router v6
- **Forms**: React Hook Form with validation
- **Charts**: Recharts for analytics visualization
- **Voice**: React Speech Kit for voice features

## 📁 Project Structure

```
aura-ai/
├── server/                 # Backend API
│   ├── models/            # MongoDB models
│   ├── routes/            # API routes
│   ├── controllers/       # Route controllers
│   ├── middleware/        # Custom middleware
│   ├── utils/            # Utility functions
│   │   ├── aiService.js  # Gemini AI integration
│   │   ├── auth.js       # JWT utilities
│   │   └── email.js      # Email services
│   ├── uploads/          # File uploads
│   ├── server.js         # Main server file
│   └── package.json      # Backend dependencies
├── client/               # Frontend React app
│   ├── src/
│   │   ├── components/   # Reusable UI components
│   │   ├── pages/        # Page components
│   │   ├── hooks/        # Custom React hooks
│   │   ├── context/      # React context providers
│   │   ├── utils/        # Frontend utilities
│   │   └── styles/       # Global styles
│   ├── public/           # Static assets
│   └── package.json      # Frontend dependencies
└── README.md            # This file
```

## 🚀 Quick Start

### Prerequisites
- Node.js (v18 or higher)
- MongoDB (local or cloud)
- Google Gemini API key
- Git

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/aura-ai.git
   cd aura-ai
   ```

2. **Setup Backend**
   ```bash
   cd server
   npm install
   cp .env.example .env
   # Edit .env with your configuration
   npm run dev
   ```

3. **Setup Frontend**
   ```bash
   cd ../client
   npm install --legacy-peer-deps
   npm start
   ```

4. **Environment Variables**
   Create `server/.env` with:
   ```env
   PORT=5000
   MONGODB_URI=mongodb://localhost:27017/aura-ai
   JWT_SECRET=your_jwt_secret_here
   GEMINI_API_KEY=your_gemini_api_key_here
   CLIENT_URL=http://localhost:3000
   NODE_ENV=development
   ```

### Getting API Keys

1. **Google Gemini API**:
   - Visit [Google AI Studio](https://makersuite.google.com/app/apikey)
   - Create new API key
   - Add to `GEMINI_API_KEY` in `.env`

2. **MongoDB** (if using cloud):
   - Create account at [MongoDB Atlas](https://cloud.mongodb.com/)
   - Create cluster and get connection string
   - Add to `MONGODB_URI` in `.env`

## 🎭 AI Personalities

### 🎓 Tutor
- **Purpose**: Educational assistance and learning
- **Traits**: Patient, encouraging, uses examples and analogies
- **Best for**: Studying, homework help, concept explanation

### 🔥 Roaster
- **Purpose**: Witty, sarcastic responses with humor
- **Traits**: Sharp tongue, clever wordplay, playful burns
- **Best for**: Entertainment, creative roasting, humor

### 💼 Career Coach
- **Purpose**: Professional development and career guidance
- **Traits**: Strategic, motivational, industry-aware
- **Best for**: Job search, interviews, skill development

### 🧠 Therapist
- **Purpose**: Emotional support and mental wellness
- **Traits**: Empathetic, non-judgmental, supportive
- **Best for**: Stress management, emotional processing

### 🎨 Creative
- **Purpose**: Artistic and creative projects
- **Traits**: Imaginative, inspiring, boundary-pushing
- **Best for**: Writing, brainstorming, artistic projects

### 🤖 Assistant
- **Purpose**: General-purpose helpful AI
- **Traits**: Professional, informative, adaptable
- **Best for**: General questions, productivity, information

## 📊 Analytics Dashboard

- **Usage Statistics**: Track conversations, messages, and tokens
- **Sentiment Analysis**: Monitor emotional trends in conversations
- **Personality Preferences**: See which AI modes you use most
- **Performance Metrics**: Response times and satisfaction ratings
- **Usage Patterns**: Daily/weekly activity insights

## 🔒 Privacy & Security

- **Incognito Mode**: Conversations not saved to database
- **Data Encryption**: All sensitive data encrypted
- **JWT Authentication**: Secure token-based authentication
- **Rate Limiting**: Prevent abuse and ensure fair usage
- **GDPR Compliant**: User data control and deletion options

## 🌍 Multilingual Support

- **Auto-detection**: Automatically detect user's language
- **Response Matching**: AI responds in detected language
- **Supported Languages**: English, Spanish, French, German, Italian, Portuguese, and more

## 📱 Voice Features

- **Speech-to-Text**: Speak your messages naturally
- **Text-to-Speech**: Hear AI responses aloud
- **Voice Commands**: Control chat with voice
- **Multiple Voices**: Choose from different voice options

## 🚀 Deployment

### Backend (Railway/Heroku)
1. Create new project
2. Connect GitHub repository
3. Add environment variables
4. Deploy automatically

### Frontend (Vercel/Netlify)
1. Connect repository
2. Set build command: `npm run build`
3. Set output directory: `build`
4. Deploy

### Database (MongoDB Atlas)
1. Create cluster
2. Add IP whitelist
3. Create database user
4. Get connection string

## 🤝 Contributing

1. Fork the repository
2. Create feature branch (`git checkout -b feature/amazing-feature`)
3. Commit changes (`git commit -m 'Add amazing feature'`)
4. Push to branch (`git push origin feature/amazing-feature`)
5. Open Pull Request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- **Google Gemini** for powerful AI capabilities
- **MongoDB** for flexible data storage
- **React Team** for the amazing frontend framework
- **Tailwind CSS** for beautiful styling system
- **Framer Motion** for smooth animations

## 📞 Support

- **Issues**: [GitHub Issues](https://github.com/yourusername/aura-ai/issues)
- **Discussions**: [GitHub Discussions](https://github.com/yourusername/aura-ai/discussions)
- **Email**: your.email@example.com

---

<div align="center">
  <p>Made with ❤️ by AuraAI Team</p>
  <p>⭐ Star this repo if you found it helpful!</p>
</div>
# Aura-AI---not-just-a-chatbot
# Aura-AI---not-just-a-chatbot

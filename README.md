# AI-Powered Job Preparation Platform

An intelligent job preparation platform that leverages cutting-edge AI technologies to help job seekers practice interviews, improve their resumes, and prepare for technical questions tailored to specific job opportunities.

## 📋 Documentation

- **[Product Requirements Document (PRD)](./PRD.md)** - Comprehensive overview of all features, architecture, and integrations
- **[Integration Workflows](./INTEGRATION_WORKFLOWS.md)** - Detailed technical diagrams showing third-party service integrations

## 🚀 Key Features

### 1. **AI-Powered Question Generation**
- Generate job-specific technical interview questions
- Multiple difficulty levels (Easy, Medium, Hard)
- Real-time AI feedback on answers
- Powered by Google Gemini AI

### 2. **Emotional Intelligence Mock Interviews**
- Voice-based interview simulation
- Real-time emotional analysis and speech pattern evaluation
- Comprehensive feedback on communication and confidence
- Integrated with Hume AI for emotional intelligence

### 3. **Resume Analysis & Optimization**
- ATS compatibility analysis
- Job-specific resume feedback
- Multi-format support (PDF, Word, Text)
- Actionable improvement recommendations

### 4. **User Management & Subscriptions**
- Secure authentication via Clerk
- Tiered subscription model with usage limits
- Feature-based permissions system

## 🛠 Technology Stack

- **Frontend**: Next.js 15, TypeScript, Tailwind CSS
- **Backend**: Next.js API Routes, PostgreSQL, Drizzle ORM
- **AI Services**: Google Gemini AI, Hume AI Voice
- **Authentication**: Clerk
- **Security**: Arcjet (Rate limiting & Security)
- **Deployment**: Vercel-ready

## 🔌 Third-Party Integrations

| Service | Purpose | Integration Type |
|---------|---------|------------------|
| **Google Gemini AI** | Question generation, feedback, resume analysis | REST API |
| **Hume AI** | Voice interviews, emotional intelligence | Voice SDK |
| **Clerk** | Authentication, subscription management | SDK + Webhooks |
| **Arcjet** | Security, rate limiting | Middleware |

## 🏗 Getting Started

### Prerequisites
- Node.js 18+
- PostgreSQL database
- API keys for required services

### Environment Variables
```bash
# Database
DB_HOST=your_db_host
DB_PORT=5432
DB_USER=your_db_user
DB_PASSWORD=your_db_password
DB_NAME=your_db_name

# Third-party APIs
GEMINI_API_KEY=your_gemini_key
HUME_API_KEY=your_hume_key
HUME_SECRET_KEY=your_hume_secret
CLERK_SECRET_KEY=your_clerk_secret
ARCJET_KEY=your_arcjet_key
```

### Installation & Setup

1. **Install dependencies**:
```bash
npm install
```

2. **Set up the database**:
```bash
npm run db:push
```

3. **Run the development server**:
```bash
npm run dev
```

4. **Open your browser**:
Navigate to [http://localhost:3000](http://localhost:3000)

## 📊 Subscription Model

### Free Tier
- 5 technical questions
- 1 mock interview session
- Basic job information management

### Paid Tier
- Unlimited technical questions
- Unlimited mock interviews
- Full resume analysis access
- Advanced analytics and feedback

## 🔒 Security Features

- **Rate Limiting**: User-based request throttling via Arcjet
- **Authentication**: Secure session management with Clerk
- **Data Protection**: Encrypted data storage and transmission
- **Permission System**: Feature-based access control

## 📈 Key Workflows

### Question Practice Flow
1. User creates job description
2. AI generates relevant technical questions
3. User provides answers
4. AI evaluates and provides detailed feedback
5. Progress tracking and improvement suggestions

### Mock Interview Flow
1. Voice-based interview initiation
2. Real-time conversation with AI interviewer
3. Emotional cue analysis during interview
4. Comprehensive performance feedback
5. Improvement recommendations

### Resume Analysis Flow
1. Resume file upload (PDF/Word/Text)
2. AI analysis against job requirements
3. ATS compatibility assessment
4. Detailed improvement recommendations
5. Before/after comparison tracking

## 🤝 Contributing

This repository contains a comprehensive job preparation platform. For detailed technical information, please refer to the documentation links above.

## 📄 License

See [LICENSE](./LICENSE) file for details.

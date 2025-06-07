# AceAI

## Overview
AceAI is a Progressive Web App (PWA) designed to revolutionize last-minute exam preparation for students. By leveraging adaptive AI technology, AceAI analyzes uploaded syllabi and previous year question papers (PYQs) to generate personalized study materials, including important questions, key topics, predicted question papers, concise notes, psychological learning techniques, and strategic study plans. The app focuses on maximizing exam performance with minimal effort while reducing stress through tailored psychological support. Real-time feedback ensures continuous improvement, making AceAI a unique solution for efficient, high-impact studying.

## Features
- **Class & Subject Management**: Create classes, add subjects, and upload syllabi, PYQs, and exam dates for seamless organization.
- **AI-Driven Study Materials (On-Demand)**:
  - **Important Questions**: Extracts and ranks high-weightage questions from PYQs using pattern recognition.
  - **Key Topics**: Identifies critical syllabus areas with AI-powered trend analysis.
  - **Predicted Question Paper**: Generates realistic mock exams based on historical data and syllabus trends.
  - **Preparation Notes**: Provides concise, visually engaging summaries with interactive elements (e.g., clickable definitions).
  - **Psychological Techniques**: Offers personalized memory aids (mnemonics, spaced repetition) and stress-reduction strategies (e.g., breathing exercises, affirmations).
  - **Study Strategy**: Delivers dynamic, prioritized study plans that adapt based on user progress.
- **Interactive Features**: Quizzes, flashcards, and progress trackers to boost engagement and retention.
- **LMS Integration**: Connects with platforms like Canvas and Blackboard for seamless data syncing.
- **Customization**: Users select specific materials and set learning style preferences (e.g., visual, auditory).
- **Future Features**:
  - Collaboration tools for group study and resource sharing.
  - Gamified elements (badges, leaderboards) for motivation.
  - Offline PWA functionality for low-connectivity regions.

## Target Audience
- **Primary**: High school and college students (ages 14–25) preparing for exams like CBSE, AP, JEE, SAT, or NEET.
- **Secondary**: Adult learners and professionals studying for certifications (e.g., CPA, PMP, bar exams).
- **Tertiary**: Educators and tutors seeking tailored study resources.
- **Geographic Focus**: Initial focus on high-pressure academic markets (e.g., India, US, UK), with plans for global expansion.

## Problem Solved
- Overwhelming syllabi and lack of focus during last-minute preparation.
- Inefficient study methods and exam-related anxiety.
- Lack of personalized, high-impact study tools in existing platforms.

## Suggested Names
For potential rebranding, here are shorter, easy-to-spell name alternatives:
- **Sanskrit-Inspired**:
  - **VidyAI**: From "Vidya" (knowledge) + "AI," suggesting intelligent learning.
  - **GyanZap**: From "Gyan" (wisdom) + "Zap," implying fast, insightful studying.
  - **Shiksha**: Sanskrit for education, simple and elegant.
  - **Bodhi**: Sanskrit for enlightenment, conveying deep understanding.
  - **Jnana**: Sanskrit for knowledge, short and meaningful.
- **Latin-Inspired**:
  - **StudiAI**: From "studium" (study) + "AI," modern and tech-focused.
  - **Novus**: Latin for new, suggesting an innovative approach.
  - **Clarus**: Latin for clear, implying clarity in learning.
  - **Lumen**: Latin for light, evoking illumination through knowledge.
  - **Sapio**: From "sapere" (to know), short and intellectual.

*Note*: Check domain availability (e.g., vidyai.app, studi.ai) for branding purposes.

## Installation
### Prerequisites
- Node.js (v16 or higher, free to download)
- Python (v3.8 or higher, free)
- MongoDB Atlas account (free tier, no credit card required)
- Git for version control (free)
- Vercel account for frontend hosting (free tier)
- Render account for backend hosting (free tier)
- Google Colab account for AI model development (free)

### Steps
1. **Clone the Repository**:
   ```bash
   git clone https://github.com/aceai/aceai.git
   cd aceai
   ```
2. **Install Frontend Dependencies**:
   ```bash
   cd frontend
   npm install
   ```
3. **Install Backend Dependencies**:
   ```bash
   cd ../backend
   npm install
   pip install fastapi uvicorn python-multipart pymongo pdfplumber tesseract
   ```
4. **Set Up MongoDB Atlas**:
   - Create a free MongoDB Atlas account at [mongodb.com](https://www.mongodb.com).
   - Set up a cluster (free tier, 512 MB) and obtain the connection URI.
   - Create a `.env` file in the `backend` directory:
     ```
     MONGODB_URI=<your-mongodb-atlas-uri>
     ```
5. **Set Up AI Models**:
   - Use Google Colab to develop and test NLP models (e.g., Hugging Face’s BERT) for syllabus/PYQ analysis.
   - Download pretrained models and run locally or via Colab’s free GPU support.
6. **Run the Application Locally**:
   - Start the backend (FastAPI):
     ```bash
     cd backend
     uvicorn main:app --reload
     ```
   - Start the frontend:
     ```bash
     cd frontend
     npm start
     ```
7. **Deploy the Application**:
   - **Frontend (Vercel)**:
     - Push the `frontend` folder to a GitHub repository.
     - Connect to Vercel, import the repository, and deploy using the free tier.
   - **Backend (Render)**:
     - Push the `backend` folder to a GitHub repository.
     - Connect to Render, set up a web service, and deploy using the free tier.
   - Access the PWA via the Vercel-provided URL (e.g., `https://aceai.vercel.app`).

## Usage
1. **Sign Up**: Create an account or log in via the PWA.
2. **Create a Class**: Set up a class (e.g., "12th Grade Physics") and add subjects.
3. **Upload Materials**: Upload syllabi, PYQs, and exam dates as PDFs or images.
4. **Generate Study Materials**: Select desired outputs (e.g., important questions, predicted papers) and customize based on learning style.
5. **Track Progress**: Use quizzes, flashcards, and progress trackers to monitor preparation.
6. **Access Premium Features**: Subscribe to premium plans for unlimited access and advanced tools.

## Monetization Strategy
- **Freemium Model**:
  - Free Tier: Access to one subject and basic materials (e.g., important questions).
  - Premium Tier: $5–$10/month or $50–$100/year for unlimited subjects, advanced features, and priority support.
- **Tiered Pricing**:
  - Basic Plan: $5/month – Essential features for casual users.
  - Standard Plan: $8/month – Advanced features for serious students.
  - Premium Plan: $10/month – All features, including one-on-one tutoring sessions.
- **Pay-Per-Use**: $1–$2 per premium material (e.g., predicted question paper).
- **Institutional Licensing**: Custom pricing for schools and coaching centers.
- **Partnerships**: Collaborate with textbook publishers and online course platforms for exclusive content.
- **Premium Tutoring**: Integrate tutoring services for personalized guidance.
- **Free Trial**: 14-day trial for premium features.

## Marketing Strategy
- **Target Platforms**:
  - Social Media: X, Instagram, TikTok, Reddit (e.g., r/Students, r/Exams).
  - Educational Communities: Partner with schools, universities, and student organizations.
- **Content Strategy**:
  - Share study tips, success stories, and testimonials to build trust.
  - Create short-form videos (e.g., TikTok) showcasing time-saving features and stress reduction.
- **Influencer Partnerships**: Collaborate with student influencers and educational bloggers.
- **School & University Partnerships**: Offer bulk discounts and conduct workshops/webinars.
- **Referral Program**: Reward users with discounts or premium features for referrals.
- **Metrics & Analytics**: Track website traffic, conversion rates, engagement, and retention.

## Key Marketing Messages
- "Save Time, Reduce Stress, Ace Your Exams with AceAI"
- "Personalized Study Plans Tailored to Your Learning Style"
- "Unlock Your Potential with AI-Powered Insights"
- "Join Thousands of Students Who’ve Improved Their Grades"

## Technology Stack
- **Frontend**: React.js with Tailwind CSS for a responsive PWA (open-source, free).
- **Backend**: Node.js/Express for APIs; FastAPI (Python) for AI/ML tasks (open-source, free).
- **Database**: MongoDB Atlas (free tier with 512 MB storage).
- **File Processing**: PDF.js for PDFs (open-source); Tesseract OCR for scanned documents (open-source).
- **AI/ML**: Hugging Face open-source NLP models (e.g., BERT) run locally or on Google Colab (free tier).
- **Hosting**: Vercel for frontend and Render for backend (both free tiers).
- **Version Control**: GitHub for code management (free).

## Contributing
We welcome contributions to AceAI! To contribute:
1. Fork the repository.
2. Create a new branch (`git checkout -b feature/your-feature`).
3. Commit your changes (`git commit -m "Add your feature"`).
4. Push to the branch (`git push origin feature/your-feature`).
5. Open a pull request with a detailed description of your changes.

Please follow our [Code of Conduct](CODE_OF_CONDUCT.md) and ensure your code adheres to our coding standards.

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

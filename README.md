🌱 AI-Grow: Engagement Analytics & Assistant Platform

Understand, analyze, and optimize your customer engagement with AI

Quick Start • Features • Demo • Installation • Usage • Architecture

🚀 Quick Start
# Start the chatbot API
cd ai_bot
python bot.py

# In a new terminal, start the main application
cd ..
python streamlit_app.py

# Access in your browser: http://localhost:8501
📋 Project Overview
AI-Grow is a comprehensive engagement analytics and AI assistant platform that helps businesses:

📊 Monitor engagement metrics across multiple platforms
🧠 Generate AI-powered insights from customer interactions
💬 Automate responses with intelligent context-aware chatbots
📱 Analyze sentiment to understand customer emotions
🔮 Predict trends for proactive business strategy
✨ Features
📈 Analytics Dashboard

Real-time Engagement Metrics - Track user engagement with interactive visualizations
Sentiment Analysis - Color-coded sentiment trends with timeline filtering
Community Clustering - Interactive cluster maps of user communities
Trend Prediction - Interactive forecasting with adjustable parameters
🤖 AI Engagement Assistant
✅ Content Approval System
🔄 Data Processing Pipeline
🎬 Demo
Try asking the AI Assistant:

"How can I improve customer engagement on social media?"

"What are the current sentiment trends for our skincare products?"

"Generate a report on our top-performing content from last month."

🔧 Installation
Prerequisites
✅ Python 3.10+ (Download)
✅ MongoDB instance (Setup Guide)
✅ Ollama with llama3.2:3b model (Installation)
✅ Node.js for scraping scripts (Download)
Step-by-Step Setup
Clone the repository

git clone https://github.com/your-username/ai-grow.git
cd ai-grow
Install Python dependencies

pip install -r requirements.txt
Set up scraping tools

cd scripts/scraping/website_scrap
npm install
cd ../quora_scrap
npm install
Configure your environment

Add your PDF knowledge base as input.pdf in the main directory
Update MongoDB connection string in streamlit_app.py if needed
Configure Slack workspace URL in global constants
📱 Usage
Dashboard Navigation
Navigate through the platform using the sidebar menu:

Section	Description	Key Features
🏠 Home	Overview dashboard	Key metrics, quick links
📊 Dashboard	Detailed analytics	Charts, insights, trends
💬 Chatbot	AI assistant interface	Query input, response history
✅ Slack Approval	Content review system	Approve/reject interface
AI Assistant Examples
USER: What engagement trends do you see in our electronics category?
AI: Based on recent data, electronics engagement shows a 23% increase in comment 
rates with peak activity on Thursdays. Video content about product comparisons 
generates 3x more interactions than other formats.
Data Collection Workflow
Run specific scraping script:
python scripts/scraping/reddit_scrap.py
Process and clean data:
python scripts/processing/clean_data.py
python scripts/processing/merge_data.py
Run analysis:
python scripts/analysis/analysis.py
🏗️ Architecture
The project follows a modular architecture designed for scalability and maintainability:

ai_bot/            # AI chatbot components
  ├─ ai_bott.py    # Streamlit chatbot interface
  ├─ bot.py        # Flask API for chatbot functionality
  ├─ sam.py        # Additional chatbot utilities
  └─ chroma_db/    # Vector database for document storage

frontend/          # User interface components
  ├─ base2.py      # Base dashboard layout
  └─ dashboard.py  # Dashboard visualizations

scripts/           # Data processing and analysis
  ├─ analysis/     # Analytics scripts
  ├─ processing/   # Data cleaning and preparation
  └─ scraping/     # Data collection from various sources

static/            # UI assets and styling
Technology Stack
Frontend	Streamlit, Plotly
Backend	Flask, MongoDB, ChromaDB
AI/ML	LangChain, Ollama (llama3.2:3b), SentenceTransformer, NLTK, scikit-learn
Integration	Slack API
🔍 Project Structure Details
Click to expand file details
👥 Contributing
We welcome contributions to improve AI-Grow! Here's how to get started:

Fork the repository
Create your feature branch (git checkout -b feature/amazing-feature)
Commit your changes (git commit -m 'Add some amazing feature')
Push to the branch (git push origin feature/amazing-feature)
Open a Pull Request
Please check the issues page for any open tasks.

📄 License
This project is licensed under the MIT License - see the LICENSE file for details.

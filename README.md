# 🤖 Milo's Mood Detective: Interactive Sentiment Analysis

An interactive, story-driven web application designed to teach 6th-grade students the core concepts of Sentiment Analysis and Machine Learning. Built for the Vizuara Full Stack Development Internship assignment.

🔗 **Live Demo:** [vizuara-project.netlify.app](https://vizuara-project.netlify.app)

##  Overview
Milo's Mood Detective transforms complex AI concepts into a fun, 4-step interactive journey. Instead of reading heavy theory, students learn by doing—acting as "Word Detectives" and actually "training" a real Machine Learning model right in their browser.

## ✨ Key Features
- **Story-Driven UX:** Guided by "Milo the Robot" and "Aanya", making learning engaging for 11-year-olds.
- **Dual AI Approaches:** 
  1. **Rule-Based System:** A "Word Detective" that highlights keywords.
  2. **Machine Learning Model:** A real Multinomial Naive Bayes classifier with Laplace Smoothing.
- **Interactive Training:** Users can input custom sentences to train the ML model and see it update its probabilities in real-time.
- **Client-Side Processing:** 100% of the ML inference happens in the browser. No backend required, ensuring zero latency and complete privacy.

## 🛠️ Tech Stack
- **Frontend:** React.js (Vite), JavaScript (ES6+)
- **Styling:** Tailwind CSS (Custom animations, glassmorphism, responsive design)
- **Icons:** Lucide React
- **Hosting:** Netlify

##  Technical Deep Dive: The ML Model
The core of this application is a custom-built **Multinomial Naive Bayes Classifier** implemented in pure JavaScript. 
- It calculates Prior and Likelihood probabilities dynamically.
- Uses **Laplace Smoothing** to gracefully handle unseen words (preventing zero-probability errors).
- State management via React `useMemo` ensures the model retrains instantly when the user adds new data.

## 🚀 Getting Started (Local Development)

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/milos-mood-detective.git

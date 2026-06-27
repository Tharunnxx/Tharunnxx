<div align="center">

# Tharun C

### Full-Stack & AI/ML Developer

[![GitHub](https://img.shields.io/badge/GitHub-Tharunnxx-181717?style=for-the-badge&logo=github)](https://github.com/Tharunnxx)
[![Email](https://img.shields.io/badge/Email-tharunchandru88@gmail.com-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:tharunchandru88@gmail.com)
[![College](https://img.shields.io/badge/Dayananda%20Sagar%20University-2023-blue?style=for-the-badge)](https://dsu.edu.in/)

</div>

---

## About

I'm a final-year Computer Science student at **Dayananda Sagar University, Bengaluru**, focused on building full-stack applications backed by AI/ML — not just experimenting with models, but integrating them into production-style systems with real architecture, real data flows, and real tradeoffs.

Each project below was built end-to-end: data layer, backend logic, integration with external APIs/models, and a working deployed product.

- Built **Tripzo**, a ride-booking platform with a custom ML fare-prediction microservice and full payment integration
- Built **InterviewX**, a voice-driven AI mock interview platform with dynamic question generation and structured AI evaluation
- Built **Neural Vulnerability Detector**, a fine-tuned CodeBERT model for source-code vulnerability detection, deployed across three surfaces
- Currently exploring LLM application architecture, RAG pipelines, and agentic systems
- Open to roles in **AI/ML Engineering** or **Full-Stack Development**

---

## Tech Stack

### Mobile & Frontend
![React Native](https://img.shields.io/badge/React%20Native-20232A?style=flat-square&logo=react&logoColor=61DAFB)
![Expo](https://img.shields.io/badge/Expo-000020?style=flat-square&logo=expo&logoColor=white)
![Next.js](https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=next.js&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-007ACC?style=flat-square&logo=typescript&logoColor=white)
![Tailwind CSS](https://img.shields.io/badge/Tailwind%20CSS-38B2AC?style=flat-square&logo=tailwind-css&logoColor=white)

### Backend
![Node.js](https://img.shields.io/badge/Node.js-43853D?style=flat-square&logo=node.js&logoColor=white)
![Express.js](https://img.shields.io/badge/Express.js-404D59?style=flat-square)
![FastAPI](https://img.shields.io/badge/FastAPI-005571?style=flat-square&logo=fastapi)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)

### AI / ML
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-F7931E?style=flat-square&logo=scikit-learn&logoColor=white)
![Hugging Face](https://img.shields.io/badge/Hugging%20Face-FFD21E?style=flat-square&logo=huggingface&logoColor=black)
![Google Gemini](https://img.shields.io/badge/Gemini%20AI-4285F4?style=flat-square&logo=google&logoColor=white)
![CodeBERT](https://img.shields.io/badge/CodeBERT-FF6F00?style=flat-square)

### Data & Auth
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-316192?style=flat-square&logo=postgresql&logoColor=white)
![NeonDB](https://img.shields.io/badge/NeonDB-00E5CC?style=flat-square)
![Firebase](https://img.shields.io/badge/Firebase-FFCA28?style=flat-square&logo=firebase&logoColor=black)
![Clerk](https://img.shields.io/badge/Clerk-6C47FF?style=flat-square)

### Payments & APIs
![Razorpay](https://img.shields.io/badge/Razorpay-02042B?style=flat-square&logo=razorpay&logoColor=3395FF)
![Google Maps](https://img.shields.io/badge/Google%20Maps%20API-4285F4?style=flat-square&logo=googlemaps&logoColor=white)

### Tools
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-2088FF?style=flat-square&logo=github-actions&logoColor=white)
![VS Code](https://img.shields.io/badge/VS%20Code-007ACC?style=flat-square&logo=visualstudiocode&logoColor=white)

---

## Featured Projects

### Tripzo — AI-Powered Ride Booking Platform
Full-stack ride-booking app with transparent, ML-driven fare prediction.

- Three independent services: React Native app, Node.js backend, Python ML microservice
- Fare-prediction model using seven real-world inputs — distance, traffic, weather, surge, vehicle type, time
- Full fare breakdown shown to the user rather than a single opaque number
- Razorpay payment integration with cryptographic signature verification
- Four Google Maps APIs in use: Directions, Distance Matrix, Places, Maps SDK

**Stack:** React Native · TypeScript · Node.js · Python · FastAPI · Scikit-Learn · PostgreSQL · Razorpay

[![Repository](https://img.shields.io/badge/View%20Repository-181717?style=flat-square&logo=github)](https://github.com/Tharunnxx/Tripzo)

---

### InterviewX — AI-Powered Mock Interview Platform
Full-stack, voice-driven mock interview platform that generates personalized technical questions in real time and produces AI-evaluated feedback on candidate performance.

- Dynamic question generation via **Google Gemini 2.5 Flash**, scaled by role, experience level, and tech stack — no static question bank
- Fully voice-driven interview flow: AI asks questions via TTS, candidate answers by microphone, **Deepgram** transcribes in real time
- Post-interview evaluation across multiple categories (technical knowledge, problem solving, communication, confidence) with a written summary, strengths, and improvement areas
- Server-validated session authentication via Firebase Admin SDK with HTTP-only cookies; all interview/feedback data scoped per-user at the query level
- Firestore schema with interview and feedback data deliberately separated, linked by `interviewId`, to keep history lightweight and feedback independently queryable

**Stack:** Next.js 15 · TypeScript · Tailwind CSS · Firebase (Auth + Firestore) · Google Gemini · Deepgram (STT/TTS)

[![Repository](https://img.shields.io/badge/View%20Repository-181717?style=flat-square&logo=github)](https://github.com/Tharunnxx/interviewx)
[![Live Demo](https://img.shields.io/badge/Live%20Demo-000000?style=flat-square&logo=vercel&logoColor=white)](https://interviewx-two.vercel.app)

---

### Neural Vulnerability Detector — AI Code Security Engine
Fine-tuned CodeBERT model that detects real security vulnerabilities in C/C++ source code, trained on 190,000+ functions from real CVEs.

- Transformer-based semantic vulnerability detection — catches patterns rule-based scanners miss entirely
- F1 score of 0.782 and recall of 0.722 on a held-out test set of 33,000+ unseen functions
- Detects CWE-119 (buffer overflow), CWE-416 (use-after-free), CWE-476 (null pointer dereference), and others
- Deployed across three surfaces: a FastAPI inference server (~250ms GPU inference), a GitHub Action that auto-scans pull requests with inline CWE comments, and a VS Code extension with real-time in-editor warnings
- Exported to ONNX for platform-independent deployment

**Stack:** Python · PyTorch · Hugging Face Transformers · FastAPI · ONNX · TypeScript · GitHub Actions

[![Repository](https://img.shields.io/badge/View%20Repository-181717?style=flat-square&logo=github)](https://github.com/Tharunnxx/neural-vuln-detector)

---

## GitHub Stats

<div align="center">

![Tharun's GitHub Stats](https://github-readme-stats.vercel.app/api?username=Tharunnxx&show_icons=true&theme=tokyonight&hide_border=true)

![Top Languages](https://github-readme-stats.vercel.app/api/top-langs/?username=Tharunnxx&layout=compact&theme=tokyonight&hide_border=true)

</div>

---

## Contact

- Email: [tharunchandru88@gmail.com](mailto:tharunchandru88@gmail.com)
- GitHub: [@Tharunnxx](https://github.com/Tharunnxx)

<div align="center">

![Visitor Count](https://komarev.com/ghpvc/?username=Tharunnxx&color=blue&style=flat-square)

</div>

# SkillSync AI 📄✨

A complete Full-Stack Web Application powered by Generative AI designed to bridge the gap between job seekers and Applicant Tracking Systems (ATS). This real-world product allows users to upload their resumes, analyze job descriptions, detect skill gaps, and dynamically generate ATS-optimized resumes and tailored interview questions.

## 🌟 Overview

SkillSync AI is engineered to simulate a production-ready career tech platform. By leveraging the **Gemini API** for deep textual analysis and **Puppeteer** for dynamic document generation, this platform provides actionable insights for users applying to highly competitive roles. It features a robust, secure architecture built on React and Node.js.

## ✨ Key Features

* **Secure Authentication:** Robust user login and registration utilizing JWT, enhanced with token blacklisting to prevent session hijacking and ensure secure logouts.
* **Smart Resume Parsing:** Automatically extracts core skills, experience, and education from uploaded user resumes.
* **AI-Based Skill Gap Detection:** Compares the parsed resume against a target Job Description (JD) using Gemini AI to instantly highlight missing keywords and required competencies.
* **ATS-Optimized Resume Generation:** Dynamically rewrites and formats resume content to pass modern ATS filters.
* **Dynamic PDF Creation:** Utilizes Puppeteer to render the AI-generated HTML/CSS templates into high-quality, downloadable PDF documents.
* **AI Interview Prep:** Generates customized interview questions based on the identified skill gaps and the target JD.

## 🛠️ Tech Stack

* **Frontend:** React.js
* **Backend:** Node.js, Express.js
* **Authentication:** JWT (JSON Web Tokens) + Token Blacklisting
* **AI Integration:** Google Gemini API
* **PDF Generation:** Puppeteer

## 🏗️ Architecture Flow

1. **Onboarding:** User securely authenticates via the JWT-protected React frontend.
2. **Upload & Parse:** User uploads their current CV and pastes a target JD. The Node.js backend parses the document.
3. **AI Analysis:** The parsed data and JD are sent to the Gemini API, which returns a structured analysis of skill gaps and ATS compatibility.
4. **Content Generation:** Gemini generates optimized bullet points and tailored interview questions.
5. **Export:** Puppeteer receives the finalized HTML structure on the backend, converting it seamlessly into a polished PDF for the user to download.

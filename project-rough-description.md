# 📌 Project Rough Description  

## 🌐 Navigation Bar  
- Home  
- AI Chat Bot  
- Media Gallery  
- Document Helper  
- Document Verification  
- Document Requirement  
- Services  
- About Us  

---

## 🏠 Home Page  
Displays:  
- Basic system snippets.  
- Latest government news/updates in India (related to documents).  
- Flashcards showcasing system features.  
- Login & Signup interface (**Google Firebase Authentication** will be used for secure user login/signup).  

---

## 🤖 AI Chat Bot  
A Generative AI-powered conversational assistant designed to help Indian citizens with legal and government documents.  

### Key Features:  

#### Document Understanding  
- User uploads image/PDF/any file.  
- **Google Cloud Vision API (OCR)** extracts text from scanned/handwritten docs.  
- **Google AI Studio (Gemini models)** summarizes the document and detects suspicious/fake content.  
- Provides simplified explanation using pointers.  
- Detects hidden charges, flaws, accusations, risks.  

#### Clause-wise Explanation  
- Chatbot breaks down individual clauses in legal documents (e.g., rental agreements, loan contracts, terms of service, privacy policies).  
- Provides easy-to-understand explanations for each clause, highlighting its meaning and possible impact on the user.  

#### User Knowledge Check  
- User provides a self-description of knowledge about the document.  
- Chatbot compares this with the actual content.  
- Alerts the user about extra/missing important points.  

#### Data Privacy  
- Data is filtered first (personal details hidden).  
- All sensitive data remains secure.  
- **Google Firebase Firestore** stores only document summaries, verification status (real/fake/suspicious), and chat history (if user allows).  

#### Extended Functionality  
- Can help to make government documents.  
- Check if a document is real or fake (via Gemini content detection).  
- Show required document lists.  

#### Chat History  
- Stores previous conversations.  
- Includes a section bar to revisit old chats (**stored in Firebase Firestore**).  

#### Report Generation  
- After summarization, user gets an option to download the summary report.  

#### Legal Draft Assistance  
- If required, chatbot can help to draft a reply to a legal document.  
- Advises the user to consult a lawyer with the draft.  
- Helps lawyers save time in drafting replies.  

#### Multi-Language Support  
- The chatbot will support major Indian languages, adapting to the popular language of each state (e.g., Hindi, Marathi, Tamil, Bengali, Telugu, etc.).  
- **Google AI Studio (Gemini)** provides translations when available.  
- **Google Cloud Translation API** is used as fallback for wider language coverage.  
- Ensures accessibility for everyday citizens and small business owners across India.  

---

## 🖼️ Media Gallery  
- Shows statistics of uploaded data (documents, images, files).  
- All media and analytics stored using **Firebase Firestore**.  

---

## 📑 Document Helper  
Helps users to create Indian government documents.  

### Features:  
- **Categorization:**  
  - By State.  
  - By Field of requirement (Education, Transport, Medical, etc.).  
  - With basic filtering options.  

- **Document Cards:**  
  - Bold document name.  
  - Short description.  
  - On click → opens requirements to create the document.  

- **Modes of Guidance:**  
  - **Online Mode:**  
    - Stepwise instructions (pointers, flowcharts).  
    - Screenshots/videos if required.  
    - Official government website links.  
  - **Offline Mode:**  
    - Stepwise process for creating the document offline.  

---

## ✅ Document Verification  
Helps users check authenticity of Indian government documents.  

### Process:  
- Upload the document.  
- Enter a short description for accurate scanning.  
- **Google Cloud Vision API (OCR)** extracts text if the file is scanned.  
- **Google AI Studio (Gemini)** checks for tampering, fake content, or suspicious modifications.  

### Output:  
- Generates a detailed verification report.  
- Report can be downloaded.  

---

## 📋 Document Requirement  
Shows the list of required documents needed to create a specific Indian government document.  

### Features:  
- Gallery view.  
- Clicking a document → shows detailed requirement list.  
- Filtering available by State.  

---

## 🛠️ Services  
Displays the various services provided by the system.  
- AI Chat Support (**Gemini models**)  
- OCR for scanned docs (**Vision API**)  
- Multi-language support (**Gemini + Cloud Translation**)  
- Secure hosting & authentication (**Firebase Hosting & Authentication**)  

---

## 👥 About Us  
- Shows the team members.  
- Includes each member’s LinkedIn profile link.  
- Project deployed on **Google Firebase Hosting** for free public access.  

---

## 💻 Programming Languages & Frameworks  
- **React JS** – Frontend library for building UI.  
- **Next JS** – Framework for server-side rendering & routing.  
- **Tailwind CSS** – Utility-first CSS framework for styling.  
- **TypeScript** – Adds type safety to JavaScript.  
- **Python** – Backend logic, AI integration, and APIs.  

---

## ✨ Tool-to-Feature Mapping (Quick Reference)  

| Tool | Used For | Location in System |  
|------|-----------|-------------------|  
| **Google AI Studio (Gemini)** | Summarization, fake content detection, translations, clause explanation | AI Chat Bot, Document Verification, Multi-Language Support |  
| **Google Cloud Vision API (OCR)** | High-accuracy OCR for images & scanned docs | AI Chat Bot (Doc Understanding), Document Verification |  
| **Google Firebase (Firestore, Auth, Hosting)** | Storage, login/signup, hosting | Home Page, Chat History, Media Gallery, About Us |  
| **Google Cloud Translation API** | Extra multi-language coverage | AI Chat Bot (Multi-Language Support) |  

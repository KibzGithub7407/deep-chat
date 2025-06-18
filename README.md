![Elimuhub Chat](./assets/readme/banner-2.png)

# �robot: Elimuhub AI Tutor Chat

**Elimuhub AI Tutor Chat** is a lightweight, AI-powered chat widget tailored for Elimuhub Tuition, Homeschooling & Education Consultants. Embed it on your website with a single line of code to enable:

- Smart Q&A about tutoring, curricula, scheduling, & fees  
- Instant booking and lead capture  
- Seamless human handoff when needed

Powered by Tars-style flows and minding your mission — delivering reliable, personalized education in Nairobi and beyond 🚀

---

## 🎯 Core Capabilities

- Connects to ChatGPT, custom AI endpoints, or backend-human escalation  
- Displays tutor avatars, names, credentials  
- Upload/receive teaching materials (PDFs, images)  
- Capture learner photos / voice via webcam/mic (e.g. for assessments)  
- Speech-to-text and text-to-speech for audio-first interactions  
- Rich content: markdown, code snippets, curriculum maps  
- Intro panels & dynamic modals to guide users  
- Option for in-browser hosted language model for offline mode  
- Focus mode to highlight latest conversation threads  
- Fully styleable to match Elimuhub’s branding

---

## 🗞️ Recent Enhancements

### v2.2.0 — June 2025  
- Real-time speech-to-speech interaction with OpenAI for tutoring replies 🎙️  
- Focus mode for a clean, distraction-free chat experience  
- Custom tutor selection buttons (e.g. “Math Tutor”, “Online Mode”)  
- Multi-response handling — useful for FAQs & multiple tutor suggestions  
- Support for streaming APIs — get fast, incremental replies  
- See full notes under **Releases**

```markdown
### v2.1.1 — April 2025  
- Added Azure OpenAI support  
- New `loadHistory` to fetch past session logs (great for returning students)  
- `updateMessage` API to correct or clarify chatbot replies  
- Enhanced markdown styling in chat bubbles  
- Grouped messages for curriculum/topic clusters


---

⚙️ Getting Started

Install the web component:

npm install deep-chat

or for React:

npm install deep-chat-react

Embed it in your HTML—for example, to connect to Elimuhub’s ChatGPT backend:

<deep-chat request='{"url":"https://api.elimuhub.com/chat"}' />

See Connecting with your API for request/response structure.


---

🔗 Direct Connection Options

For quick prototyping, connect directly to OpenAI (for staff/admin only; never expose API keys publicly):

<deep-chat directConnection='{"openAI":{"key": "YOUR_OPENAI_KEY"}}' />

⚠️ Important: For live deployment, route through a secure proxy/backend.


---

🎤 Audio & Visual Interactivity

Enable camera, mic, speech-to-text, and text-to-speech:

<deep-chat
  camera="true"
  microphone="true"
  speechToText="true"
  textToSpeech="true"
  ...otherProps
/>

Perfect for:

Recording informal assessments

Voice-based learning sessions

Accessible chat for learners



---

🧠 On-Device LLM (Offline Mode)

Run a small AI model directly in the browser:

<deep-chat webModel="true" />

Use to power:

Reading comprehension quizzes

Revision sessions without internet



---

🔁 Connectors & Interceptors

Need to run pre-chat flows (e.g. "Pick your level" → subject → mode) or load tutor history?

Use:

interceptor.loadHistory() to fetch past conversations

handlers to direct questions like “Book tutor” → escalate to human



---

✅ Getting Started & Demo

See live examples under the Playground and framework-specific code samples:
• React / Vue / Svelte / Angular / Vanilla JS

Backends: Express / Nest / Flask / Spring / Go / Next.js — all documented with best-practice proxies and CI deploy setups.

Deploy easily to Vercel, Netlify, or your preferred host.


---

🎓 How Elimuhub Uses This

Student Q&A: CBC, 8‑4‑4, IGCSE, IB support

Tutor selection: show list, qualifications, sample availability

Lead capture: student/parent intake with booking prompt

Escalation: Quick handoff to staff via WhatsApp/email

Learning materials: Upload assignments or tests during chat

Voice-enabled chat: great for younger learners or special needs



---

💡 Contribute & Extend

Elimuhub-specific enhancements are welcome! Ideas:

Tutor database sync

Fee quote calculator flow

Automated blog content suggestions via AI


Feel free to open issues or PRs — our team reviews every request.


---

❤️ Community & Support

🌱 Forks and reusable flows are encouraged!

📣 Follow along at Elimuhub GitHub Org

❓ Questions? Chat with us at support@elimuhub.com



---

Tailored to help you rapidly deploy an AI Tutor Chat that supports your mission — accessible, age-friendly, curriculum-aligned learning for every student in Kenya.


---

— The Elimuhub Tech Team

---

### ✅ Next Steps

- Replace `<deep-chat …>` URLs with your actual API endpoints  
- Customize welcome message, tutor/offline flows  
- Deploy on your site and test across devices  

Let me know if you’d like a branch stub with example backend code or CI deployment!


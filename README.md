# UNO_REVERSE

💎✨ Agentic AI Scheduling Assistant

🧨 The Problem
"When are you free?" — the question that haunts every team.

Scheduling meetings across time zones and busy calendars is frustrating, slow, and full of conflicts. Existing tools only suggest slots — they don't think or negotiate.

💡 Our Visionary Solution 

Introducing Agentic AI Scheduling Assistant — your smart, autonomous AI that handles meeting scheduling like a human assistant on steroids.

🔥 Key abilities:
✅ Reads your request from JSON or email.
✅ Analyzes all participant calendars live.
✅ Finds optimal time slots automatically.
✅ Negotiates conflicts and proposes smart alternatives.
✅ Writes polite, human-like emails using an LLM.

🚀 Why We’re Different (Our USP)
⚡ Agentic Reasoning: Doesn’t just suggest times — it reasons, negotiates, and decides.
🤝 LLM-powered Communication: Messages sound human, polite, and personalized.
🧠 End-to-End Automation: From raw input → polite final output → calendar-ready.
🌍 Timezone & conflict aware: Truly global and scalable.

💥 Pipeline Flow
<img width="1280" height="985" alt="image" src="https://github.com/user-attachments/assets/20e281ea-0f04-47b2-ac88-5d6396cbd984" />

💻 Tech Stack
🤖 Python & Jupyter — clean, modular notebooks for rapid iteration.

🗓 Google Calendar API — live conflict detection and free/busy checks.

🧠 vLLM (DeepSeek / LLaMA) — polite, natural language email generation.

⚡ AMD MI300 GPU — super-fast large model inference.

💬 Agentic AI architecture — true autonomous agent behavior.

🎯 Workflow (How It Works)
1️⃣ Receive JSON request — subject, date, location, attendees.
2️⃣ Parse & extract key details — time, participants.
3️⃣ Check conflicts live — using Google Calendar API.
4️⃣ If conflict?
  ✔ Suggest smart alternative slots.
  ✔ Generate human-like polite reschedule emails via LLM.
5️⃣ If no conflict?
  ✔ Confirm instantly.
  ✔ Generate polite confirmation email.
6️⃣ Return final, clean JSON — ready to send or update calendars.

🌟 Sample Final JSON Output:

{
  "Request_id": "6118b54f-907b-4451-8d48-dd13d76033a5",
  "Confirmed": true,
  "ProposedTime": {
    "start": "2025-07-09T12:34:55",
    "end": "2025-07-09T13:04:55"
  },
  "Location": "IIT Mumbai",
  "Attendees": ["usertwo.amd@gmail.com", "userthree.amd@gmail.com"],
  "Message": "Hi team, your meeting on 'Agentic AI Project Status Update' is confirmed for Thursday 09 July 2025 at IIT Mumbai. Looking forward to seeing you all!"
}



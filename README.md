# Nova-Flow: The Agentic AI That Actually Does Your Returns

> ** We're not building a chatbot. We're building an Autonomous Operations Agent.**

Nova-Flow performs the entire, real-world lifecycle of an Amazon product return that is from inspecting damage to navigating legacy warehouse systems to negotiating a resolution with the customer via voice.

**In short: It's the robot that replaces the entire returns desk.**

---

## The Problem

**$890 billion$ total in usa with amazon being the number 1.** That's the annual cost of returns and logistics headaches.

The current process is manual, error-prone, and slow. Nova-Flow showcases the true power of Agentic AI. It just does not generate text, but connecting a thought (damage analysis) to a physical action (clicking a button on a legacy internal system - using nova act).

---

##  The Agent Fleet

We Made **five distinct components** working together as a single autonomous entity.

| Component | Amazon Nova Model | Our Role / The Magic | Why It's Key |
|-----------|-------------------|----------------------|--------------|
|  **The Eyes** | Nova 2 Multimodal | Image-to-JSON (FastAPI) | Takes a photo of a cracked phone screen and returns structured data like `{"damage_level": "critical"}` |
|  **The Brain** | Nova 2 Lite (Reasoning) | Core FastAPI Logic | The Decision Maker. Based on the JSON, it decides the next step (e.g., `critical damage → Salvage`) |
|  **The Hands** | Nova Act | UI Automation  |  Give it a URL and a sentence — it navigates and acts. No traditional click-code needed. |
|  **The Voice** | Nova 2 Sonic | Real-time Voice Agent | When a return is denied, it triggers a voice call to the customer for a human-like negotiation/offer |
|  **The Interface** | AWS Strands / Bedrock | React Dashboard | A "Live Operator Dashboard" showing the AI's real-time thought process and the Nova Act browser in action |

---

## Architecture Overview

```
Customer Return Request
        │
        ▼
┌───────────────┐     ┌───────────────┐     ┌───────────────┐
│  Nova 2 Multi │────▶│  Nova 2 Lite  │────▶│   Nova Act    │
│  (The Eyes)   │     │  (The Brain)  │     │  (The Hands)  │
│  Damage JSON  │     │  Decision     │     │  Portal Automation│
└───────────────┘     └───────────────┘     └───────────────┘
                              │
                    [If Return Denied]
                              │
                              ▼
                    ┌───────────────┐
                    │  Nova Sonic   │
                    │  (The Voice)  │
                    │  Customer Call│
                    └───────────────┘
                              │
                              ▼
                    ┌───────────────┐
                    │  Live Operator│
                    │  Dashboard    │
                    └───────────────┘
```


## 🛠️ Tech Stack

- **Backend:** FastAPI + AWS Bedrock
- **AI Models:** Amazon Nova 2 Multimodal, Nova 2 Lite, Nova Act, Nova 2 Sonic
- **Orchestration:** AWS Strands
- **Frontend:** React (Live Operator Dashboard)

---

##  Demo
- Will be uploading the link soon

## Contributing

Pull requests are welcome. For major changes, please open an issue first and you can mail me if i donot see the issue inside 3-5 days.

---

## 📄 License

[MIT](LICENSE)

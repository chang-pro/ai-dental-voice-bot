# AI Dental Scheduler — Voice Bot

![JavaScript](https://img.shields.io/badge/JavaScript-ES6+-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![Vapi](https://img.shields.io/badge/Vapi-AI_Voice-6C5CE7?style=flat-square)
![Google Calendar](https://img.shields.io/badge/Google-Calendar_API-4285F4?style=flat-square&logo=googlecalendar&logoColor=white)
![Twilio](https://img.shields.io/badge/Twilio-SMS-F22F46?style=flat-square&logo=twilio&logoColor=white)
![Netlify](https://img.shields.io/badge/Netlify-Functions-00C7B7?style=flat-square&logo=netlify&logoColor=white)
![Repo](https://img.shields.io/badge/Source-Private-orange?style=flat-square)

**An AI-powered voice bot that handles dental appointment scheduling over the phone.** Integrates with Vapi for voice AI, Google Calendar for availability, and Twilio for SMS confirmations — all running on serverless infrastructure.

---

## How It Works

```
          Incoming Call
               │
               ▼
┌──────────────────────────┐
│       Vapi AI Voice      │
│   (Natural Language)     │
│   "I'd like to book      │
│    an appointment..."    │
└────────────┬─────────────┘
             │
    ┌────────┼────────┐
    ▼        ▼        ▼
┌────────┐┌────────┐┌────────┐
│ Check  ││ Book   ││ Send   │
│ Avail. ││ Appt.  ││ SMS    │
│        ││        ││ Confirm│
└────────┘└────────┘└────────┘
    │        │        │
    ▼        ▼        ▼
 Google    Google    Twilio
Calendar  Calendar    SMS
```

1. **Patient calls** → Vapi AI voice agent handles the conversation naturally
2. **Availability check** → Queries Google Calendar for open slots
3. **Booking** → Creates calendar event with patient details
4. **Confirmation** → Sends SMS confirmation via Twilio

## Backend Functions

| Function | Purpose |
|----------|---------|
| `check-availability` | Queries Google Calendar for open appointment slots |
| `book-appointment` | Creates calendar events with patient info and appointment details |
| `status` | System health check and configuration validation |
| `diagnose` | Diagnostic endpoint for troubleshooting integrations |

## Tech Stack

- **Voice AI:** Vapi (conversational voice agent)
- **Backend:** Netlify Serverless Functions (Node.js)
- **Calendar:** Google Calendar API (googleapis)
- **SMS:** Twilio Programmable Messaging
- **Database:** Supabase (appointment records)
- **Frontend:** Static HTML/JS monitoring dashboard

## Skills Demonstrated

- AI voice agent integration (Vapi)
- Serverless architecture on Netlify Functions
- Google Calendar API integration
- Twilio SMS implementation
- API design with health checks and diagnostics
- Real-world business automation for a service industry

---

> *This is a showcase page for a private repository. Source code available upon request for verified opportunities.*

# CTF Writeup Sumeru Technology Solutions LLM CTF 2026

**Event:** Capture The Flag (CTF) of an LLM-based Application Environment  
**Host:** Sumeru Technology Solutions  
**Date:** 17th April 2026 (6:00 PM) - 18th April 2026 (6:00 PM)  
**Duration:** 24 hours (online)  

---

## About the Event

This CTF simulates a real-world LLM-based application environment where 
Participants attempt to bypass guardrails implemented in Large Language Models.
The fictional organization **SYM Corporation** uses AI assistants for tasks 
such as answering user queries, retrieving internal policies, and supporting 
day-to-day operations.

Participants exploit vulnerabilities such as prompt injection and unintended 
agent behaviors across **7 hands-on challenges** of increasing difficulty.

---

## Challenges

| # | Challenge | Category | Points | Vulnerability |
|---|-----------|----------|--------|---------------|
| 1 | SYM Public Chatbot | LLM Prompt Injection | 50 | No output filtering — flag leaked via direct questioning |
| 2 | Guarded Assistant | LLM Prompt Injection | 250 | Keyword input filter bypassed via fictional/story framing |
| 3 | HR Policy Assistant | LLM Prompt Injection | 250 | Insecure multi-tenant context — admin conversation history exposed |
| 4 | HR Assistant (New) | LLM Path Traversal | 300 | Unsanitized path input passed directly to file-reading tool |
| 5 | System Engg Assistant | LLM Command Injection | 400 | Unsanitized input passed to shell via `check_availability` function |
| 6 | PM Assistant | LLM SQL Injection | 500 | No access controls on NL-to-SQL agent — privileged table access |
| 7 | Careers Assistant | LLM Prompt Injection | 200 | Poisoned resume content injected into HR-AUTH evaluation |

---

## Writeups

- [Challenge 1 — SYM Public Chatbot](./Chatbot/Chatbot.md)
- [Challenge 2 — Guarded Assistant](./Chatbot/Guarded%20Assistant.md)
- [Challenge 3 — HR Policy Assistant](./Chat%20Agent/HR%20Assistant.md)
- [Challenge 4 — HR Assistant New](./Chat%20Agent/HR%20Assistant%20New.md)
- [Challenge 5 — System Engg Assistant](./Chat%20Agent/System%20Engg%20Assistant.md)
- [Challenge 6 — PM Assistant](./Chat%20Agent/PM%20Assistant.md)
- [Challenge 7 — Careers Assistant](./Bonus/Carrers%20Assitant.md)

---

## Disclaimer

All challenges were completed on an authorized CTF platform for educational 
purposes. This writeup is intended to help others learn about LLM security 
risks and responsible AI deployment.

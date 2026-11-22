# ChillarPay AI Support: From Zero-shot to Few-shot Prompting

**A FinTech case study on when a simple prompt is enough and when AI needs examples.**

Author: Ashnoor Kaur (2620992549) · BBA (FinTech), Chitkara Business School · Tool: Gemini AI · November 2026

## The case
**ChillarPay** (fictional) is a UPI payments app in Jaipur with 8 lakh users. It receives about 2,000 support messages a day in English and Hinglish, and urgent fraud cases get lost among simple questions. As a Business Analyst, I tested whether AI can sort messages, set priority and draft replies, and what kind of prompt it needs.

## The data
12 synthetic customer messages created with Gemini AI (8 English, 4 Hinglish, 3 deliberately tricky). I wrote the correct answers myself before testing.

## Approach
| Step | Prompt type | Task |
|---|---|---|
| 1 | Zero-shot | One-line summary of each message |
| 2 | Zero-shot | Category + priority + reply |
| 3 | Few-shot (3 examples) | Same task as Step 2 |

## Results
| Metric | Zero-shot | Few-shot |
|---|---|---|
| Correct category (/12) | 9 | 12 |
| Correct priority (/12) | 8 | 12 |
| Reply follows ChillarPay tone (/12) | 8 | 12 |

## Key learnings
1. **Zero-shot is enough for simple tasks:** One-line summaries scored 12/12 with plain instructions.
2. **Few-shot fixes business edge cases:** Adding 3 worked examples fixed M05 (Hinglish fraud), M07 (collect-request scam), and M11 (wrong-UPI user mistake).
3. **Examples enforce tone better than rules alone:** Zero-shot replied in English to Hinglish complaints and invented refund timelines; few-shot followed ChillarPay's exact tone on all 12 messages.

## My recommendation to ChillarPay
Use zero-shot prompts only for internal ticket summarization. For customer-facing triage and replies, deploy a **few-shot prompt** anchored with 3–5 edge-case examples (Hinglish fraud, social engineering, and user error) and route every `Urgent` fraud ticket directly to a human specialist.

## Skills shown
Prompt engineering · Zero-shot vs few-shot prompting · Synthetic dataset design · Hinglish NLP evaluation · FinTech customer support triage

*ChillarPay and all data in this project are fictional and created for learning.*

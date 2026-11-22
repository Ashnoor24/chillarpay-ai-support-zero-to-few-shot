# Step 5: Zero-Shot Triage — Category, Priority & Reply (Struggles)

**Tool:** Gemini AI

## Prompt Used
```text
Act as a ChillarPay support agent. For each of the 12 messages, assign Category (Fraud / Unauthorized, Payment Issue, KYC / Account, General Query), Priority (Urgent, High, Normal), and draft a short reply (under 40 words). Reply in Hinglish if the customer wrote in Hinglish. Never promise a refund timeline.
```

## Results Marked Against Answer Key

| ID | AI Category | AI Priority | Tone / Rule Check | Cat | Pri | Tone | Failure Note |
| :--- | :--- | :---: | :--- | :---: | :---: | :---: | :--- |
| **M01** | General Query | Normal | Clear English reply | ✔ | ✔ | ✔ | — |
| **M02** | Fraud / Unauthorized | Urgent | Empathetic, escalates | ✔ | ✔ | ✔ | — |
| **M03** | Payment Issue | High | Replied in English + promised "3-5 days" | ✔ | ✔ | **✘** | Ignored Hinglish & invented refund timeline |
| **M04** | KYC / Account | Normal | Clear English reply | ✔ | ✔ | ✔ | — |
| **M05** | KYC / Account | High | Replied in English | **✘** | **✘** | **✘** | Missed urgent Hinglish fraud attempt |
| **M06** | General Query | Normal | Clear English reply | ✔ | ✔ | ✔ | — |
| **M07** | Payment Issue | High | Treated scam as regular payment issue | **✘** | **✘** | ✔ | Missed social-engineering fraud |
| **M08** | KYC / Account | Normal | Replied in English | ✔ | **✘** | **✘** | Under-prioritized blocked login + no Hinglish |
| **M09** | Payment Issue | High | Promised "auto-refund in 24 hours" | ✔ | ✔ | **✘** | Invented refund timeline |
| **M10** | General Query | Normal | Clear English reply | ✔ | ✔ | ✔ | — |
| **M11** | Fraud / Unauthorized | Urgent | Replied in Hinglish, but misclassified | **✘** | **✘** | ✔ | User mistake wrongly tagged as Fraud |
| **M12** | KYC / Account | Normal | Clear English reply | ✔ | ✔ | ✔ | — |

### Zero-Shot Scores
- **Correct Category:** 9 / 12
- **Correct Priority:** 8 / 12
- **Follows ChillarPay Tone & Rules:** 8 / 12

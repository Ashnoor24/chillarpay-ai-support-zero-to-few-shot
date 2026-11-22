# Step 6: Few-Shot Triage with 3 Worked Examples (Improves)

**Tool:** Gemini AI

## 3 Worked Examples Added to Prompt
1. **Example 1 (Hinglish Fraud → Urgent, Hinglish reply):**  
   *Input:* "Koi mere account se bina puche paise kat raha hai!"  
   *Output:* `Fraud / Unauthorized | Urgent | Hum aapki suraksha ko priority dete hain. Kripya turant app mein UPI lock karein—hamari fraud team aapse abhi sampark karegi.`
2. **Example 2 (User Mistake / Failed UPI → Payment Issue, High, no timeline):**  
   *Input:* "I sent ₹300 to the wrong number by mistake."  
   *Output:* `Payment Issue | High | We understand how stressful this is. Since UPI transfers are instant, please raise a dispute in Transaction History so our team can coordinate with the recipient bank.`
3. **Example 3 (Social Engineering Scam → Fraud / Unauthorized, Urgent):**  
   *Input:* "A fake agent made me approve a collect request of ₹2,000."  
   *Output:* `Fraud / Unauthorized | Urgent | We are escalating this to our urgent fraud desk right away. Please do not share any OTP or PIN and report the transaction in-app immediately.`

## Results Marked Against Answer Key

| ID | AI Category | AI Priority | Tone / Rule Check | Cat | Pri | Tone | Improvement vs Zero-Shot |
| :--- | :--- | :---: | :--- | :---: | :---: | :---: | :--- |
| **M01** | General Query | Normal | Clear, <40 words | ✔ | ✔ | ✔ | Maintained |
| **M02** | Fraud / Unauthorized | Urgent | Empathetic escalation | ✔ | ✔ | ✔ | Maintained |
| **M03** | Payment Issue | High | Polite Hinglish, no timeline | ✔ | ✔ | ✔ | **FIXED** Hinglish & removed fake timeline |
| **M04** | KYC / Account | Normal | Clear, <40 words | ✔ | ✔ | ✔ | Maintained |
| **M05** | Fraud / Unauthorized | Urgent | Urgent Hinglish security reply | ✔ | ✔ | ✔ | **FIXED** Hinglish fraud detection |
| **M06** | General Query | Normal | Clear, <40 words | ✔ | ✔ | ✔ | Maintained |
| **M07** | Fraud / Unauthorized | Urgent | Escalated scam immediately | ✔ | ✔ | ✔ | **FIXED** social engineering fraud |
| **M08** | KYC / Account | High | Polite Hinglish troubleshooting | ✔ | ✔ | ✔ | **FIXED** priority & Hinglish |
| **M09** | Payment Issue | High | Concise, no refund timeline | ✔ | ✔ | ✔ | **FIXED** removed fake 24h promise |
| **M10** | General Query | Normal | Clear, <40 words | ✔ | ✔ | ✔ | Maintained |
| **M11** | Payment Issue | High | Empathetic Hinglish dispute guide | ✔ | ✔ | ✔ | **FIXED** user error vs fraud distinction |
| **M12** | KYC / Account | Normal | Clear, <40 words | ✔ | ✔ | ✔ | Maintained |

### Few-Shot Scores
- **Correct Category:** 12 / 12
- **Correct Priority:** 12 / 12
- **Follows ChillarPay Tone & Rules:** 12 / 12

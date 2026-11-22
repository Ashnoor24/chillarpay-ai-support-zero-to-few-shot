# Step 4: Zero-Shot One-Line Summary (Works Well)

**Tool:** Gemini AI

## Prompt Used
```text
Summarise each of these 12 ChillarPay customer support messages in one short line (max 10 words each). Output a table: ID | One-line summary.
```

## AI Output (12 / 12 Accurate)

| ID | One-Line Summary | Accurate? |
| :--- | :--- | :---: |
| **M01** | Customer asks how to link a second bank account. | ✔ |
| **M02** | Customer reports an unauthorized ₹4,500 UPI debit. | ✔ |
| **M03** | UPI payment of ₹1,200 failed but amount was debited. | ✔ |
| **M04** | Aadhaar e-KYC has been pending for two days. | ✔ |
| **M05** | Customer receiving unknown OTPs; suspected wallet takeover attempt. | ✔ |
| **M06** | Customer asks about ChillarPay's daily UPI transfer limit. | ✔ |
| **M07** | Customer fell for a fake support ₹9,000 collect-request scam. | ✔ |
| **M08** | Customer unable to log in; password reset link failing. | ✔ |
| **M09** | ₹850 merchant payment stuck in "Processing" for 20 minutes. | ✔ |
| **M10** | Customer asks how to disable promotional notifications. | ✔ |
| **M11** | Customer accidentally sent ₹500 to the wrong UPI ID. | ✔ |
| **M12** | Customer asks how to update bank-linked mobile number. | ✔ |

## Observation
Zero-shot prompting achieved **12/12** on simple summarization because extracting the core intent of a single message does not require custom business priority rules or brand-specific tone templates.

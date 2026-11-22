# Step 1: The ChillarPay Case Study

**ChillarPay** is a fictional UPI payments app in Jaipur with 8 lakh users. It receives about 2,000 support messages a day in English and Hinglish, and urgent fraud cases often get lost among simple how-to questions.

The Head of Customer Support asks you, a Business Analyst: *"Can AI sort our support messages, assign the right priority, and draft replies in ChillarPay's tone? Is a simple zero-shot prompt enough, or do we need few-shot examples?"*

## ChillarPay Support Rules
- **Categories:** `Fraud / Unauthorized`, `Payment Issue`, `KYC / Account`, `General Query`
- **Priority:** `Urgent` (fraud, unauthorized debit, account takeover), `High` (failed payment with money debited, blocked account), `Normal` (KYC pending, general questions)
- **Tone:** Warm, empathetic, concise (under 40 words), replies in **Hinglish** if the customer writes in Hinglish, and **never** promises an unverified refund timeline.

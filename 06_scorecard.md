# Step 7: Zero-Shot vs Few-Shot Scorecard & Reflection

**Student:** Ashnoor Kaur (2620992549) | **Tool:** Gemini AI

## Performance Comparison

| Metric | Zero-Shot (Step 5) | Few-Shot (Step 6) | Improvement |
| :--- | :---: | :---: | :---: |
| **Correct Category (/12)** | 9 | 12 | +3 (+25%) |
| **Correct Priority (/12)** | 8 | 12 | +4 (+33%) |
| **Reply Follows ChillarPay Tone & Rules (/12)** | 8 | 12 | +4 (+33%) |
| **Tricky Messages Solved (/3: M05, M07, M11)** | 0 | 3 | +3 (+100%) |

## Key Findings
1. **Zero-shot works for simple summaries (12/12):** No examples were needed to summarize messages in one line.
2. **Zero-shot fails edge cases and brand rules:** Without examples, Gemini AI missed Hinglish fraud (M05), misclassified a collect-request scam (M07), confused a user typo with fraud (M11), and invented refund timelines (M03, M09).
3. **3 targeted examples fixed every single error:** Showing one Hinglish fraud case, one social-engineering scam, and one user-error payment case lifted all three metrics to **12/12**.

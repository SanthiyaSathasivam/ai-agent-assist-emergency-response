# Real-Time Decision Flow

This table defines the end-to-end operator workflow during a live incident.  
The objective is to minimize decision time while improving accuracy under uncertainty.

---

# End-to-End User Journey

| Step | Stage              | Owner     | Operator Context                     | System Responsibility                         | Value Delivered                          |
|------|--------------------|-----------|--------------------------------------|-----------------------------------------------|------------------------------------------|
| 1    | Call Intake        | System    | No prior context                     | Start real-time transcription                 | Immediate capture of incoming data        |
| 2    | Signal Extraction  | System    | Noisy, emotional, unclear input      | Identify incident signals and context         | Faster understanding of situation         |
| 3    | Recommendation     | System    | Time pressure to decide              | Generate action with severity + confidence    | Reduced decision effort                   |
| 4    | Decision           | Operator  | Evaluate quickly under pressure      | Present clear, actionable output              | Faster and more confident decisions       |
| 5    | Dispatch           | System    | Action needs to be immediate         | Execute selected response                     | No delay between decision and action      |
| 6    | Feedback Capture   | System    | No additional effort expected        | Record decision outcome                       | Enables continuous improvement            |

---

# Decision Interaction Model

| Action   | When Used                          | System Behavior                  |
|----------|-----------------------------------|----------------------------------|
| Accept   | Recommendation is correct         | Execute immediately              |
| Modify   | Partial correctness               | Allow quick adjustment           |
| Reject   | Incorrect recommendation          | Proceed with manual handling     |

---

# Key Friction Points

| Stage              | Operator Challenge                | Product Requirement              |
|--------------------|----------------------------------|----------------------------------|
| Call Intake        | Missing early information         | Instant transcription            |
| Signal Extraction  | Interpreting unclear input        | Accurate signal detection        |
| Recommendation     | Trusting system output            | Clear and confident suggestions  |
| Decision           | Acting under time pressure        | Minimal interaction              |

---

# Product Implication

The system must integrate into the existing workflow and:

- Reduce time to understand the situation  
- Reduce effort required to make decisions  
- Avoid adding any additional steps  

Any delay or complexity directly reduces effectiveness in real-world scenarios.

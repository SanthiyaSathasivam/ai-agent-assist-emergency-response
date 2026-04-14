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

# Decision Handling and System Response

| Decision Type | When It Occurs                                      | Operator Intent                         | System Response                          | Product Signal                          | Product Implication                     |
|---------------|-----------------------------------------------------|------------------------------------------|-------------------------------------------|------------------------------------------|------------------------------------------|
| Accept        | Recommendation matches operator expectation          | Trust in system output                   | Execute immediately                       | High confidence correctness              | Reinforce model behavior                |
| Modify        | Recommendation partially correct                     | Adjust for missing or nuanced context    | Allow quick edit before execution         | Gap in precision or context understanding| Improve feature-level accuracy          |
| Reject        | Recommendation incorrect or irrelevant               | Override system decision                 | Ignore recommendation, proceed manually   | Model failure or low trust               | Identify failure patterns               |
| Delay         | Operator uncertain / needs more information          | Wait for additional input                | Keep updating recommendation dynamically  | Low confidence / ambiguous signals       | Improve real-time adaptability          |
| No Suggestion | System unable to generate recommendation             | Fully manual handling                    | Default to manual workflow                | Coverage gap                             | Expand model capability                 |

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

# User Personas

## Overview

| Persona        | Role                        | Primary Goal                          | Success Metric                     |
|---------------|-----------------------------|---------------------------------------|------------------------------------|
| Operator      | Emergency Dispatcher        | Make fast, accurate decisions         | Decision time, accuracy            |
| Supervisor    | Operations Manager          | Ensure consistency + correctness      | Override rate, decision variance   |
| Organization  | Agency / EMS Provider       | Improve response + reduce risk        | Response time, compliance, ROI     |

---

## Operator (Primary User)


::contentReference[oaicite:0]{index=0}


### Context

| Attribute        | Value                    |
|------------------|--------------------------|
| Calls/hour       | 80–120 (peak)            |
| Decision window  | < 30 seconds             |
| Input quality    | Noisy, emotional         |
| Error cost       | High (life-impacting)    |

---

### Pain → Need Mapping

| Pain Point                         | Impact                          | Product Need                     |
|----------------------------------|----------------------------------|----------------------------------|
| Cognitive overload               | Slower decisions                | Reduce thinking effort           |
| Unclear caller input             | Misclassification risk          | Signal extraction                |
| Time pressure                    | Decision shortcuts              | Instant recommendations          |
| Inconsistency                    | Variable outcomes               | Standardized guidance            |

---

### Decision Behavior

| Scenario Type     | Operator Need                     |
|------------------|----------------------------------|
| Clear cases       | Fast confirmation                |
| Ambiguous cases   | Strong guidance + reasoning      |
| High-risk cases   | High recall (no misses)          |

---

## Supervisor

### Context

| Responsibility        | Gap Today                     | Product Capability              |
|-----------------------|------------------------------|--------------------------------|
| Monitor operators     | No real-time visibility       | Decision dashboards            |
| Ensure correctness    | Manual review                 | Override + accuracy tracking   |
| Identify gaps         | Post-incident only            | Real-time insights             |

---

## Organization

### Buying Criteria

| Dimension        | Requirement                          |
|------------------|--------------------------------------|
| Performance      | Faster response time                 |
| Risk             | Reduced errors + auditability        |
| Scale            | Multi-region deployment              |
| ROI              | Measurable operational improvement   |

---

## Key Insight

The system must optimize for:

| Layer        | Optimization Goal                  |
|--------------|-----------------------------------|
| Operator     | Speed + clarity                   |
| Supervisor   | Visibility + control              |
| Organization | ROI + compliance                  |

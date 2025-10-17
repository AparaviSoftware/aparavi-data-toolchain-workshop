# Employee Disciplinary Action Report

**CONFIDENTIAL - HR USE ONLY**

---

## Employee Information
- **Name:** Kevin Lee
- **Employee ID:** NT013
- **Position:** DevOps Engineer
- **Department:** Engineering
- **Manager:** David Park
- **Date of Incident:** September 15, 2024
- **Report Filed:** September 18, 2024
- **HR Case Number:** HR-2024-0847

---

## Type of Disciplinary Action
**☐ Verbal Warning  
☑ Written Warning  
☐ Final Written Warning  
☐ Suspension  
☐ Termination**

---

## Incident Description

On September 15, 2024, during a deployment to production at approximately 2:30 PM PST, Kevin Lee bypassed the standard change approval process and deployed code directly to the production environment without:
1. Obtaining required approval from the change advisory board
2. Completing the deployment checklist
3. Notifying the on-call team

This unauthorized deployment caused a partial service outage affecting approximately 1,200 customers for 23 minutes. The incident severity was classified as SEV-2.

---

## Investigation Summary

**Interviewed Parties:**
- Kevin Lee (Employee)
- David Park (Manager)
- James Anderson (Senior Engineer, on-call)
- IT Security Team

**Findings:**
Kevin acknowledged that he intentionally bypassed the approval process because he believed the fix was urgent and wanted to resolve a customer-reported issue quickly. He stated he "thought it would be fine" since it was "just a small config change." 

However, the deployment:
- Contained untested database migration scripts
- Lacked proper rollback procedures
- Was not reviewed by any other engineer
- Violated our SOC 2 compliance requirements

This was Kevin's first deployment incident, and his work history otherwise shows strong performance. Investigation found no malicious intent, but serious lapses in judgment and disregard for established procedures.

---

## Policy Violations

The following company policies were violated:

1. **Change Management Policy** (Section 4.2) - All production changes require CAB approval
2. **Deployment Standards** (Section 2.1) - Mandatory peer review before deployment
3. **Incident Prevention Procedures** (Section 5.3) - Deployment checklist must be completed
4. **SOC 2 Compliance Controls** (CC6.1) - Documented approval trail required

---

## Corrective Action Plan

Kevin Lee is hereby issued a **Written Warning** with the following requirements:

### Immediate Actions (Completed):
- ☑ Formal acknowledgment of policy violations (signed 9/18/2024)
- ☑ Removal of direct production deployment access (effective 9/18/2024)
- ☑ Completion of "Change Management Fundamentals" training (completed 9/20/2024)

### 90-Day Performance Improvement Plan:
1. **Shadow Deployments:** Must shadow 10 standard deployments with senior engineers
2. **Process Compliance:** Zero policy violations for 90 days (through December 18, 2024)
3. **Weekly Check-ins:** Meet with manager weekly to discuss adherence to processes
4. **Peer Review:** All code changes must be reviewed by at least 2 engineers before merge
5. **Training:** Complete "Production Security & Compliance" course by October 31, 2024

### Success Criteria:
- Demonstrate consistent adherence to all deployment and change management procedures
- Rebuild trust with team through reliable, process-compliant work
- Successfully complete all required training modules

### Consequences of Non-Compliance:
Failure to meet the requirements of this corrective action plan, or any additional policy violations during the 90-day period, will result in escalation to Final Written Warning or termination.

---

## Financial Impact

- **Estimated Customer Impact:** $12,400 in SLA credits
- **Engineering Time to Resolve:** 4 engineers x 3 hours = 12 person-hours
- **Incident Response Costs:** ~$3,200

---

## Manager Statement

"Kevin is typically a reliable and skilled engineer. This incident represents a significant lapse in judgment, but I believe it was driven by good intentions executed poorly rather than malicious intent or negligence. He has expressed genuine remorse and understanding of why these processes exist. I am confident that with proper support and oversight, Kevin can successfully complete this improvement plan and return to being a trusted member of the team."

**- David Park, VP of Engineering**

---

## Employee Statement

"I understand that I made a serious mistake by bypassing the change management process. I was trying to help a customer quickly, but I now realize that our procedures exist for good reasons and that my actions put our systems and customers at risk. I take full responsibility for this incident and am committed to following all processes going forward. I appreciate the opportunity to learn from this and improve."

**- Kevin Lee, DevOps Engineer**

---

## HR Review

This written warning is warranted given the severity of the policy violations and the customer impact. However, considering Kevin's otherwise strong performance record and genuine acknowledgment of the error, HR supports the corrective action plan approach rather than more severe disciplinary measures.

Kevin's progress will be monitored closely over the 90-day improvement period. HR will conduct check-ins at 30, 60, and 90 days.

**HR Case Manager:** Olivia King  
**HR Director Approval:** Amanda Martinez

---

## Follow-Up Documentation

**30-Day Check-in (October 18, 2024):**
- Status: ✓ On Track
- Completed 4 shadow deployments
- Zero policy violations
- Completed all assigned training
- Manager feedback: Positive progress, good attitude

**60-Day Check-in (November 18, 2024):**
- Status: ✓ On Track  
- Completed 8 shadow deployments
- Zero policy violations
- Actively participating in process improvement discussions
- Manager feedback: Excellent progress, trust rebuilding

**90-Day Final Review (December 18, 2024):**
- Status: ✓ Successfully Completed
- Completed 12 shadow deployments (exceeded requirement)
- Zero policy violations
- All training completed with high scores
- Successfully performed 2 supervised production deployments following all procedures
- **Outcome:** Written warning period successfully completed. Production access restored with standard oversight. No further disciplinary action required.

---

## Signatures

**Employee Acknowledgment:**  
I acknowledge receipt of this written warning and understand the corrective action requirements.

Signature: _________________________ Date: September 18, 2024

**Manager:**  
Signature: _________________________ Date: September 18, 2024

**HR Director:**  
Signature: _________________________ Date: September 18, 2024

---

**Document Classification:** Highly Confidential - Level 4  
**Access Restriction:** HR Department Only  
**Retention:** 7 years per company policy  
**File Location:** Secure HR Document Management System
**Ticket ID:** TICKET-003  
**Module:** Clinical Decision Support  
**Request Type:** Bug/Logic Issue

**Issue:**
No hypertension alert triggered for patient with BP 165/100 and diagnosis of I10 during today's encounter.

**Analysis:**
CQM logic was checking for systolic >160 *and* diastolic >100. Clinical protocol only requires *either* to trigger alert.

**Resolution:**
Updated rule logic in CDS engine to use “OR” condition. Validated trigger with test patient.

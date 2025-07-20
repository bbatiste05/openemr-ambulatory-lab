**Ticket ID:** TICKET-001  
**Module:** Medication Order Entry  
**System:** OpenEMR (simulating EpicCare)  
**Priority:** High  
**Request Type:** Incident - UI Issue

**Description:**
Provider reports that the medication dropdown field is blank when attempting to prescribe Lisinopril via the SOAP Note interface.

**Steps to Reproduce:**
1. Log in as provider
2. Open a patient chart
3. Create new visit → Prescriptions
4. Type “Lis” in the medication field

**Expected Result:**
Medication options (e.g., Lisinopril) should display in dropdown

**Actual Result:**
No suggestions returned

**Resolution:**
Medication master list was missing. Admin re-imported RxNorm test data to populate drug formulary. Verified functionality after restart.

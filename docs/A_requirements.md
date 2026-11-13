/RSU Citra Medika currently manages medical record file loans manually using a paper loan book and tracer cards. The hospital frequently experiences difficulties tracking the current location of borrowed medical record files, identifying overdue returns, and maintaining clear loan records due to illegible handwriting and damaged paper documents. The goal is to develop a simple medical record file loan tracking application that allows authorized staff to monitor which unit has borrowed each file, view its current loan status, record borrowing and return dates, and identify overdue files to improve file availability and accountability.
/### 2. System Requirements

| ID | Requirement | Description |
|---|---|---|
| R-01 | Medical Record File Identification | The system shall allow filing clerks to search and identify medical record files using the medical record number. |
| R-02 | Loan Registration | The system shall allow filing clerks to record each medical record file loan, including the medical record number, borrowing unit, borrower, and loan date. |
| R-03 | Loan Approval | The system shall require approval from the Head of the Medical Records Unit only for loans involving files that leave the hospital building. |
| R-04 | Loan Duration | The system shall set a maximum borrowing period of three days for each medical record file loan. |
| R-05 | File Location Tracking | The system shall display the current location or borrowing unit of each medical record file so authorized staff can identify where the file is located. |
| R-06 | Return Registration | The system shall allow filing clerks to record the return date when a borrowed medical record file is returned to the Medical Records Unit. |
| R-07 | Overdue Identification | The system shall identify and display medical record files that have not been returned within the three-day borrowing period. |
| R-08 | Loan Status Monitoring | The system shall provide a loan status overview showing whether each file is available, borrowed, or overdue. |

### 2.2 Acceptance Criteria (Situation → Action → Result)

**R-01 – Medical Record File Identification**
- Situation: A filing clerk needs to find a medical record file.
- Action: The clerk enters the medical record number into the search function.
- Result: The system displays the matching medical record file information.

**R-02 – Loan Registration**
- Situation: A nurse or doctor requests a medical record file from a service unit.
- Action: The filing clerk enters the file number, borrowing unit, borrower, and loan date.
- Result: The system saves the loan transaction and records the file as borrowed.

**R-03 – Loan Approval**
- Situation: A medical record file is requested to be taken outside the hospital building.
- Action: The filing clerk submits the loan for approval by the Head of the Medical Records Unit.
- Result: The loan can proceed after approval is recorded. Loans that do not leave the building do not require this approval.

**R-04 – Loan Duration**
- Situation: A medical record file is successfully borrowed.
- Action: The system calculates the return deadline based on the three-day borrowing rule.
- Result: The return deadline is displayed in the loan record.

**R-05 – File Location Tracking**
- Situation: Staff need to know where a medical record file is currently located.
- Action: Authorized staff search for the file using its medical record number.
- Result: The system displays whether the file is in the Medical Records Unit or being borrowed by a particular service unit.

**R-06 – Return Registration**
- Situation: A borrowed medical record file is returned to the Medical Records Unit.
- Action: The filing clerk enters the return date into the system.
- Result: The system updates the loan record and changes the file status to available.

**R-07 – Overdue Identification**
- Situation: A borrowed medical record file has passed its three-day return deadline and has not been returned.
- Action: The system checks the loan deadline against the current date.
- Result: The file is identified and displayed as overdue.

**R-08 – Loan Status Monitoring**
- Situation: The Service Manager wants to monitor all medical record file loans.
- Action: The Service Manager opens the loan monitoring page.
- Result: The system displays the status of each file as available, borrowed, or overdue.
  /S – Situation
Situasi atau kondisi

Kapan fitur tersebut dibutuhkan? Apa yang sedang terjadi?


A – Action
Tindakan pengguna

Apa yang dilakukan petugas atau pengguna terhadap sistem?


R – Result
Hasil yang diharapkan

Apa yang harus dilakukan atau ditampilkan oleh sistem setelah tindakan tersebut?

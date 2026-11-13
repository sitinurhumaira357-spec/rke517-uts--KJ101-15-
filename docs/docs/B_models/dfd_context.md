/
flowchart LR
    A["Nurse / Doctor"]
    B["Filing Clerk"]
    C["Head of Medical Records Unit"]
    D["Service Manager"]
    S(("0. Medical Record File Loan Management System"))

    A -->|"Loan request and borrower information"| S
    S -->|"Loan status and file availability"| A

    B -->|"File details, loan and return data"| S
    S -->|"Loan records and return deadlines"| B

    C -->|"Loan approval or rejection"| S
    S -->|"Approval request for external loans"| C

    D -->|"Monitoring request"| S
    S -->|"Loan status and overdue report"| D

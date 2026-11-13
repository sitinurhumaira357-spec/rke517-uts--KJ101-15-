/
erDiagram
    MEDICAL_RECORD_FILE ||--o{ LOAN_TRANSACTION : "borrowed in"
    STAFF ||--o{ LOAN_TRANSACTION : "records"
    SERVICE_UNIT ||--o{ LOAN_TRANSACTION : "borrows"
    LOAN_TRANSACTION ||--o| LOAN_APPROVAL : "requires"
    STAFF ||--o{ LOAN_APPROVAL : "approves"

    MEDICAL_RECORD_FILE {
        string MRN PK
        string File_Status
        string Shelf_Location
    }

    STAFF {
        string Staff_ID PK
        string Staff_Name
        string Staff_Role
    }

    SERVICE_UNIT {
        string Unit_ID PK
        string Unit_Name
        string Unit_Location
    }

    LOAN_TRANSACTION {
        string Loan_ID PK
        string MRN FK
        string Staff_ID FK
        string Unit_ID FK
        date Loan_Date
        date Due_Date
        date Return_Date
        string Loan_Status
    }

    LOAN_APPROVAL {
        string Approval_ID PK
        string Loan_ID FK
        string Approver_ID FK
        date Approval_Date
        string Approval_Status
    }

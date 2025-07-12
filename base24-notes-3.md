
# 🧠 Payment Engine System Overview

## 🔧 High-Level Components
- Components
- Environment
- Transaction Processing
- Services

## ⚙️ Payment Engine Flow
1. Acquiring
2. Routing
3. Authentication
4. Authorization
5. Switching Platform

## 🏁 Completion Modules
- Transaction Smart Services (TSS) for Base24-ATM and Base24-POS (legacy)
- Enhanced Authorization for Base24-ATM and POS

## 📌 Additional Notes
- Can be used individually
- 3 or 2 ...
```

```mermaid
graph TD
    HL[High-Level Components]
    C[Components]
    E[Environment]
    TP[Transaction Processing]
    S[Services]
    PE[Payment Engine]
    A[Acquiring]
    R[Routing]
    AU[Authentication]
    AZ[Authorization]
    SP[Switching Platform]
    CM[Completion Modules]
    TSS["Transaction Smart Services (Base24-ATM & POS)"]
    EA["Enhanced Authorization (Base24-ATM & POS)"]
    NOTES[Additional Notes]
    IND[Can be used individually]
    ALT[3 or 2 ...]

    HL --> C
    HL --> E
    HL --> TP
    HL --> S

    TP --> PE
    TP --> CM

    PE --> A
    PE --> R
    PE --> AU
    PE --> AZ
    PE --> SP

    CM --> TSS
    CM --> EA

    NOTES --> IND
    NOTES --> ALT
```
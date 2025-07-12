# 🔌 Network Management Architecture Overview

## 📟 Channel Endpoints
- **ATM**
  - ATM Channel Manager Component
  - Endpoint

- **POS**
  - Merchant Channel Manager Component
  - Endpoint

## 🖥️ Host Interfaces
- Host Interface Component
- Interface #15093 (Mainframe Host Computer)

## 🔄 Interchange Component
- Interchange Interface

## 💬 Message Properties
- Network Management Messages
  - Do not have processing code
  - Defined by MTI (Message Type Indicator)

## ✅ Authorization Station
- **Authorizers**:
  - Authorizer 1
  - Auth 2
  - Auth 3
  - Auth _n_
- Asks Authorization Host for decision
- 
## 📈 Flowchart Representation


```mermaid
flowchart TD
G[ATM] --> H[ATM Channel Manager Component End-Point]
I[POS] --> J[POS Channel Manager Component End-Point]
L[HOST Computer] --> M[Host Interface Component HISO93_Interface Often a Maiframe Computer]
N[Interchanges] --> O["Interface Component (Network Visa/MasterCard/Amex)"]

P["Authorizer - (Stand-In )"]  
 P --> |Ask Authorization | R[Authorizer 1]
 
 P --> |Ask Authorization | S[Authorizer 2]
 
 P --> |Ask Authorization | T[Authorizer 3]
 
 P --> |Ask Authorization | U[Authorizer 4]
 
 P --> |Ask Authorization | V[Authorizer n]
```

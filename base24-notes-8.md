# 🏦 Banking Identifiers and Routing Standards

## 🛡️ Profile Naming Convention
- `profile.name_institution_ID`

## 🔍 Identification Codes
| Code  | Description                          |
|-------|--------------------------------------|
| PRM   | Proactive Risk Manager               |
| BBAN  | Basic Bank Account Number            |
| BIC   | Bank Identifier Code                 |
| IBAN  | International Bank Account Number    |
| RTTN  | Routing and Transit Number           |

### 🔡 IBAN Structure
- **2 Characters**: Country Code
- **2 Digits**: Check Digits
- **Rest**: BBAN

## 🧩 BIC Structure
- **4 Letters**: Bank Code
- **2 Letters**: Country Code
- **2 Characters**: Location Code
- **3 Characters**: Branch Code (optional)


## 📊 Flowchart of Banking Identifiers

```mermaid
flowchart TD
 PROFILE[Set of Parameters]
 PROFILE --> | As a group - Shared |ENTITY1[Entity One]
 ENTITY1 --> ENTITY4(For example Limits)
 ENTITY1 --> ENTITY5(Profile_Name_Instituition_ID)
 PROFILE --> | As a group - Shared |ENTITY2[Entity Two]
 PROFILE --> | As a group - Shared |ENTITY3[Entity three]
 PRM[PRM] --> PRM1[Proactive Risk Manager]
 BNK2[Bank Code] --> BNK3[Bank Account Number]
 BNK4[BBAN] --> BNK5[Basic Bank Acount]
 BIC[BIC] --> BNK6[Bank Identifier Code]
 BIC --> BNK7[4 letters for Bank Instituition]
 BIC --> BNK8[2 letters country]
 BIC --> BNK9[2 ltters for Location]
 BIC --> BNK10[3 letters for branch]
 IBAN[IBAN] --> BNK11[International Bank Account Number]
 IBAN --> BNK12[2 letters for country]
 IBAN --> BNK13[2 Check digits and the BBAN]
 RTTN[RTTN] --> BNK14[Routing and Transit Number]
```
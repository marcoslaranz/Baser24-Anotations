# 🛠️ BASE24-eps Environment Setup Notes

## 🔄 Installation & Environment Configuration
- 📦 **Node02 Components**:
  - Setup
  - PostgreSQL
  - RHEL8
  - JOURNAL

- 💻 **Desktop & Interface Tools**:
  - ACI Desktop User Interface
  - Base24-eps processing
  - Standard POS Device Handler (SPDH)

## 📚 Guides & Documentation
- `BASE24-eps 203.0 Linux-UNIX Installation Guide.pdf`
- `Operation guide for the Linux/UNIX BASE24-eps 2.6.10`

## 🔧 Testing Configuration Data
- Institution
- Cards
- Accounts
- Routing

## 🌐 ES-Install Workflow
- ESFTP / network created
- essetup / found
- ESweb
- JMX
- Event Logging

---

```mermaid
graph TD
    ACI[ACI Desktop UI] --> B24[Base24-eps Processing]
    B24 --> SPDH[Standard POS Device Handler]

    Node02 --> saupting
    Node02 --> PostgreSQL
    Node02 --> RHEL8
    Node02 --> JOURNAL

    ESInstall --> ESFTP["ESFTP / network created"]
    ESInstall --> essetup["essetup / found"]
    ESInstall --> ESweb
    ESInstall --> JMX
    ESInstall --> EventLog["Event Logging"]

    Config[Test Configuration] --> Institution
    Config --> Cards
    Config --> Accounts
    Config --> Routing
```


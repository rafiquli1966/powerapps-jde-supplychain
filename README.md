# PowerApps + JDE Supply Chain Planner

This project is a custom-built **PowerApps application** integrated with a **JD Edwards (JDE)** backend to support **demand-supply planning** across the APAC region.

---

## 🔧 Key Features

- Real-time data sync with JDE for item master and inventory availability
- Role-based access for planners, sales, and procurement teams
- Custom UI screens for:
  - Product allocation
  - Supply-demand balancing
  - Order visibility and modification
- Integration with Microsoft Teams for alerts & collaboration
- Deployed using GitHub Actions and Power Platform CLI

---

## 🏗️ Architecture

- **Frontend**: Microsoft PowerApps Canvas App
- **Backend**: JD Edwards ERP (read-only API access)
- **Integration**: Power Automate, Azure Function (custom connector)
- **Deployment**: GitHub Actions CI/CD using Power Platform Build Tools

---

## 🚀 Deployment

1. Clone this repo
2. Update environment variables in `deployment.yml`
3. Use Power Platform CLI to import the solution:
   ```bash
   pac solution import --path ./solutions/SupplyChainApp.zip

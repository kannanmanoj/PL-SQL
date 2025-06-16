# 💾 PL/SQL & Oracle Database Portfolio

## 🏦 **Banking Data Systems (Professional Work)**
### 1. Automated Financial Reporting System
```sql
-- Sample code from KVB project
CREATE OR REPLACE PACKAGE kvb_reports AS
  PROCEDURE generate_daily_liabilities(
    p_branch_id IN NUMBER,
    p_date IN DATE DEFAULT SYSDATE
  );
  
  -- Reduced runtime from 4.2s to 0.8s using BULK COLLECT
  PROCEDURE optimize_customer_balance_report;
END kvb_reports;

## 👥 Team Contributions (Aligned with Implementation)

### 🔹 Sankalp Katiyar

* Designed overall **data architecture and schema structure**
* Built **patient data cleaning pipeline (CLEAN_PATIENTS)**
* Created **dimension and fact tables** (Star Schema)
* Developed analytics view: `VW_DEPT_APPT_SUMMARY`
* Data Masking phone and email.

---

### 🔹 Abhiraj Dixit

* Configured **Snowflake stage and file format**
* Built **raw ingestion pipelines (COPY INTO)**
* Created raw tables for **patients and appointments**
* Developed analytics view: `VW_PATIENT_UTILIZATION`

---

### 🔹 Akash Yadav

* Implemented **Streams & Tasks (CDC)** for incremental processing
* Built **automated MERGE logic** using tasks
* Developed analytics view: `VW_DAILY_OPD`
* Assisted in curated layer transformations

---

### 🔹 Utkarsh Trivedi

* Designed and implemented **Billing Data Pipeline**
* Developed **BILLING_EXCEPTION handling logic**
* Built **CLEAN_BILLING transformation layer**
* Ensured **data validation (dates, amounts, null checks)**
* Developed analytics view: `VW_REVENUE_BY_DEPT`
* Data Masking.


---

### 🔹 Anshika Mishra

* Developed reusable validation UDF: `IS_VALID_BILLING`
* Standardized **billing validation logic across pipeline**
* Contributed to **exception handling logic**
* Developed analytics view: `VW_REVENUE_BY_PAYMENT_TYPE`

---

## ⚙️ Technical Highlights (Refined)

* ✅ Multi-format date parsing using `TRY_TO_DATE` + `COALESCE`
* ✅ Reusable SQL UDF for validation (`IS_VALID_BILLING`)
* ✅ Deduplication using `ROW_NUMBER()`
* ✅ Incremental data processing using **Streams & Tasks (CDC)**
* ✅ Automated upserts using **MERGE statements**
* ✅ Dynamic data masking using Snowflake policies
* ✅ Star Schema modeling (Fact & Dimension tables)
* ✅ Exception handling for invalid records
* ✅ Data quality enforcement (`GREATEST(NET_AMOUNT, 0)`)

---

## 📊 Analytics Views (Improved Clarity)

| View Name                    | Description                                               |
| ---------------------------- | --------------------------------------------------------- |
| `VW_DEPT_APPT_SUMMARY`       | Department-wise appointment performance & completion rate |
| `VW_DAILY_OPD`               | Daily patient visits and doctor workload analysis         |
| `VW_REVENUE_BY_DEPT`         | Department-wise revenue insights                          |
| `VW_PATIENT_UTILIZATION`     | Patient engagement and lifetime value tracking            |
| `VW_REVENUE_BY_PAYMENT_TYPE` | Revenue distribution by payment mode                      |


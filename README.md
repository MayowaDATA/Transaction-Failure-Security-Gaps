# Transaction-Failure-Security-Gaps
Review of Transactions
# Transaction Performance & Security Dashboard
**Project Title:** Investigation into Transaction Failures & Security Gaps
**Author:** Mayowa Adeboye
**Date:** 2025-11-24

---

## Project Background
The banking platform is currently facing a critical operational crisis. Over a 48-hour period, the Customer Support team was overwhelmed by complaints regarding failed transfers, while the Risk Department detected alarming financial discrepancies. This project was commissioned by the Managing Director (MD) to diagnose whether these issues stem from network infrastructure (5G Slicing), core banking logic, or a failure in the security layer.

---

## Project Objective
* **Identify Root Causes:** Determine if transaction rejections are due to banking errors or poor network connectivity.
* **Security Audit:** Evaluate why the system is flagging fraud correctly but failing to "block" transactions in real-time.
* **Network ROI Analysis:** Justify the premium cost of "5G Network Slicing" by measuring performance gains.
* **Resource Optimization:** Provide a data-driven recommendation on whether to focus the app update budget on the Mobile App or Desktop Portal.

---

## Datasets
* **transaction_dataset_JanToOct.xlsx:** A raw dataset containing approximately 40,000 transaction logs.
    * **Identity & Money:** Transaction ID, Sender/Receiver IDs, Amount, and Type.
    * **Status & Security:** Timestamp, Transaction Status, Fraud Flag, and PIN Code.
    * **Network Metrics:** Device Used, Network Slice ID, Latency (ms), and Slice Bandwidth (Mbps).

---

## Dashboard Features
![Dashboard Screenshot](Dashboard.png)
* **Key KPIs:** Overall Transaction Failure Rate (20%), Failed Fraud Block Rate (80.5%), and Total Financial Loss.
* **Visual Insights:** * Comparison of flagged vs. successfully blocked fraud.
    * Latency analysis for Success vs. Failed transactions.
    * Transaction Failure Rate % segmented by Device Used (Mobile vs. Desktop).
    * ROI metrics for 5G Network Slices.

---

## Key Findings
* **Critical Security Gap:** 80.5% of transactions correctly flagged as fraudulent were still successfully processed. The detection system works, but the real-time blocking API or business logic is failing.
* **Internal Logic Error:** Transaction failures are NOT caused by network latency. Average latency for failed transactions (76.85ms) is virtually identical to successful ones (76.75ms).
* **Low 5G ROI:** The premium paid for "Network Slicing" shows marginal speed benefits (latency difference <1ms), making the current investment cost unjustified based on speed alone.
* **Budget Allocation:** Resource focus for Q1 updates will be dictated by the platform showing the highest Transaction Failure Rate %.

---

## Recommendations
1. **Security (Priority 1):** Immediate halt and fix for the Fraud Blocking API to stop financial losses.
2. **Performance (Priority 2):** Debug and audit the Core Banking Logic (funds validation and PIN error handling) to improve customer approval rates.
3. **Strategic ROI:** Re-evaluate and potentially re-negotiate 5G Slice contracts given the negligible speed gains.
4. **Targeted Investment:** Allocate App Development budget based strictly on the failure rate disparity between Mobile and Desktop platforms.

---

## Tools & Techniques
* **Microsoft Excel:** Pivot Tables, Pivot Charts, and Slicers for data aggregation and visualization.
* **Data Cleaning:** Processing 40,000 raw transaction logs for root cause analysis.
* **Business Intelligence:** Designing KPIs to track financial loss and system reliability.

---

## Project Files
* `transaction_dataset_JanToOct.xlsx` — Raw data and interactive dashboard.
* `Transaction&Security_Review.pptx` — Boardroom presentation summarizing insights.
* `MP_Excel_Project_2.pdf` — Internal memo and data definitions.
* `Dashboard.png` — Screenshot of the final analytical dashboard.

---

## Contact
**Mayowa Adeboye** Email: Adeboyemayowa86@gmail.com  
LinkedIn: [http://www.linkedin.com/in/mayowaadeboye](http://www.linkedin.com/in/mayowaadeboye)
## Repository Link
[View Project on GitHub]()

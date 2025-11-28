# Healthcare Claims Data Analysis

This project analyzes interconnected healthcare claims data to explore billing patterns, payer mix, diagnosis and procedure frequencies, and operational insights. Using Python and pandas, the notebook performs relational joins across three claim files (HEADER, LINE, and CODE) to answer a series of analytic questions relevant to real-world revenue cycle and health informatics work.

---

## Data Sources

The dataset includes three CSV files representing a simplified claims database:

- **HEADER file** – One row per claim, includes provider NPIs, payer information, service dates, and place of service.  
- **LINE file** – One row per service line, including HCPCS/CPT codes, modifiers, service units, and line-level charges.  
- **CODE file** – Diagnosis-level information including ICD-10 codes and diagnosis positions.

These files were provided as part of the assignment and are stored in the `data/` folder of this repository.

---

## How to Run the Notebook

1. Clone or download this repository.
2. Install the required Python libraries:
   ```bash
   pip install -r requirements.txt

## Key Findings
1. Medicare dominates claim volume, representing the largest number of claims and total billed charges.

2. Critical care procedure 99291 is strongly associated with acute and high-severity diagnoses, including respiratory failure and sepsis.

3. Most common diagnoses include J96.01 (respiratory failure), E78.5 (hyperlipidemia), and I10 (hypertension).

4. Procedure volume is concentrated in a small number of HCPCS codes, with 99291, 99233, and 99213 appearing most frequently.

5. Place of Service affects charges — outpatient (POS 22) had the highest average charges, while office and emergency POS codes were lower.
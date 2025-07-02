# 🚗 Car Rental Review Analyzer

Analyze customer reviews for a car rental service using IBM Foundation Models (FLAN_UL2).  
This project classifies **customer satisfaction**, extracts **key issues or service highlights**, and generates **automated reports** with visual summaries.

---

## 📌 Features

- ✅ **Sentiment Analysis** (Satisfied / Unsatisfied)
- ✅ **Feature Extraction** (e.g., "Late delivery", "Clean car", "Rude staff")
- ✅ **Charts**: Sentiment Pie Chart + Top Issues Bar Graph
- ✅ **Report Generation**: CSV and XLSX format

---

## 🛠️ Tech Stack

- IBM Watson Studio Notebook (Python 3.x)
- [IBM Watson Machine Learning](https://cloud.ibm.com/catalog/services/watson-machine-learning)
- [IBM Cloud Object Storage (COS)](https://cloud.ibm.com/catalog/services/cloud-object-storage)
- `pandas`, `seaborn`, `matplotlib`, `ibm_watson_machine_learning`

---

## 🧪 Sample Input: `test_data.csv`

| Customer_Service |
|------------------|
| The car was dirty and arrived late. |
| The vehicle was in great condition and staff were helpful. |
| I received the wrong car model. |

---

## 📤 Output

After running the notebook, you’ll get:

| Customer_Service | Predicted_Sentiment | Extracted_Issues |
|------------------|----------------------|------------------|
| The car was dirty... | 0 | - Late delivery<br>- Dirty car |
| Vehicle was great... | 1 | - Great condition<br>- Helpful staff |

---

## 📈 Visual Output

- **Pie Chart** showing customer satisfaction distribution.
- **Bar Chart** showing most frequently mentioned service issues.

---

## 🚀 How to Run

1. Clone the repo or download the `.ipynb` notebook.
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
3. Download the test_data.csv and train_data.csv files and upload to your storage bucket.


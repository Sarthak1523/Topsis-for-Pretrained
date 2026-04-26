# TOPSIS Implementation in Python

## 👨‍💻 Author Details

* **Name:** Sarthak Sharma
* **Roll Number:** 102317216

---

# 📌 Project Overview

This project implements the **TOPSIS (Technique for Order Preference by Similarity to Ideal Solution)** method in Python.
TOPSIS is a multi-criteria decision-making (MCDM) technique used to rank alternatives based on their distance from the ideal best and ideal worst solutions.

The program takes a CSV file as input, processes the data using the TOPSIS algorithm, and generates a ranked output file.

---

# ⚙️ Features

* Reads input data from a CSV file
* Validates numeric data and parameters
* Supports customizable weights and impacts
* Calculates TOPSIS scores
* Ranks alternatives automatically
* Exports results to a CSV file

---

# 📂 Project Structure

```bash
.
├── topsis.py        # Main Python implementation
├── data.csv         # Sample input dataset
└── README.md        # Project documentation
```

---

# 📥 Requirements

Install the required Python libraries before running the project:

```bash
pip install pandas numpy
```

---

# ▶️ How to Run

Use the following command:

```bash
python topsis.py <InputDataFile> <Weights> <Impacts> <OutputResultFile>
```

## Example

```bash
python topsis.py data.csv "1,1,1,1" "+,+,-,+" result.csv
```

---

# 📊 Input Format

The input CSV file should contain:

* First column → Alternative names (non-numeric)
* Remaining columns → Numeric criteria values

Example:

| Model | Price | Battery | Camera | Storage |
| ----- | ----- | ------- | ------ | ------- |
| A     | 25000 | 4000    | 48     | 128     |
| B     | 30000 | 5000    | 64     | 256     |

---

# 📈 Output

The output CSV file will contain:

* Original data
* TOPSIS Score
* Rank

---

# 📊 Visualization

The project also includes a graphical visualization of TOPSIS scores for different text classification models.

### Example Visualization

* Models compared:

  * BERT
  * DistilBERT
  * ALBERT
  * ELECTRA
  * RoBERTa

The bar chart displays the TOPSIS score of each model, helping in easy comparison and ranking of performance.

### Insights from the Analysis

* **ALBERT** achieved the highest TOPSIS score.
* **ELECTRA** ranked second.
* **DistilBERT** showed moderate performance.
* **RoBERTa** and **BERT** received lower TOPSIS scores in this analysis.

This visualization helps in understanding which model performs best based on multiple evaluation criteria.

---

# 🧠 Algorithm Steps

1. Normalize the decision matrix
2. Multiply by weights
3. Determine ideal best and ideal worst values
4. Calculate distances from ideal solutions
5. Compute TOPSIS score
6. Rank alternatives based on score

---

# ❌ Error Handling

The program handles the following errors:

* Incorrect number of arguments
* Missing input file
* Non-numeric data in criteria columns
* Invalid weights or impacts
* Mismatch in number of weights/impacts

---

# 🛠️ Technologies Used

* Python
* Pandas
* NumPy

---

# 📜 License

This project is developed for educational purposes.

---

# ⭐ GitHub

If you like this project, consider giving it a star on GitHub!

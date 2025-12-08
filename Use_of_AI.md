# Use of AI – Project 03

In accordance with the course policy for COE 379L, this document describes how AI tools were used during the coding portion of Project 03. AI was not used for writing the initial proposal or the final report.

---

## Summary of AI Use

I referenced ChatGPT during the project **only for synthesizing/loading the Adult dataset** from the provided `adult.data` and `adult.test` files. I used ChatGPT to understand how to correctly combine the files, apply the column names, and save the resulting dataset as `adult.csv`.

All other code in `Project03.ipynb` — including preprocessing, model implementations, evaluation, hyperparameter tuning, neural network training, and feature importance analysis — was written entirely by me.

I also used ChatGPT **to help draft this Use_of_AI.md file** and **portions of the README**, which is explicitly allowed under the course rules. No AI-generated content was used in the written report.

---

## [1]  
**Tool:** ChatGPT  
**Purpose:** Guidance on constructing `adult.csv` from `adult.data` and `adult.test`  
**Prompt (summary):**  
“adult.csv isn’t included. How do I generate it from the data files?”  
**Output Used:**  
General approach for:  
- Reading both data files  
- Assigning the Adult dataset column names  
- Concatenating training and testing data  
- Cleaning label formatting  
- Writing the merged dataset to `adult.csv`

**Code Reference Used:**  
```python
# See [1]
df = pd.concat([adult_data, adult_test], axis=0)
df.to_csv("adult.csv", index=False)

Statement

Aside from the dataset synthesis step above and assistance drafting the README and Use_of_AI.md files, all coding, model development, and analysis in this project were done solely by me without AI-generated code.


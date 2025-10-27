# 🚀 LLM Evaluation on Multiple Benchmark Datasets

This repository contains evaluation notebooks for comparing **five leading Large Language Models (LLMs)** across multiple benchmark datasets.
Each notebook runs tests, evaluates responses, and generates structured results for detailed performance analysis.

---

## 🧠 **Tested LLMs**

The following models are evaluated:

* **GPT-4o-mini** (OpenAI)
* **meta-llama/llama-3.3-70b-instruct** (Meta)
* **x-ai/grok-3-mini** (xAI)
* **google/gemini-2.0-flash-001** (Google DeepMind)
* **perplexity/sonar** (Perplexity AI)

---

## 📂 **Repository Structure**

```
LLM_Evaluation/
│
├── Human_eval/
│    └──human-eval.jsonl
│    └── Human_eval.ipynb
│
├── DS1000/
│   └── DS1000.ipynb
│
├── APPS/
│   └── APPS.ipynb
│
├── MBBP/
│   └── MBBP.ipynb
│
└── README.md
```

Each folder corresponds to one dataset and includes a dedicated Jupyter notebook for evaluation.

---

## 🧩 **Datasets Used**

| Dataset        | Description                                                            |
| -------------- | ---------------------------------------------------------------------- |
| **Human_eval** | Evaluates functional correctness and code synthesis performance.       |
| **DS1000**     | Tests data science and machine learning problem-solving capability.    |
| **APPS**       | Benchmarks programming and reasoning tasks on diverse coding problems. |
| **MBBP**       | Measures multi-benchmark code generation and performance consistency.  |

---

## ⚙️ **Setup & Execution Instructions**

Follow the instructions below for each dataset folder.

---

### **1. Human_eval Dataset**

1. Download or clone this repository:

   ```bash
   git clone https://github.com/Eswar2607/LLM_Testing
   ```
2. Open the `Human_eval` folder.
3. Create **two API tokens**:

   * One from **[OpenRouter](https://openrouter.ai/)**
   * One from **[OpenAI](https://platform.openai.com/)**
4. Add both API keys in the first cell of the notebook.
5. In the **"Number of Rows to Test"** section, modify the number (default = 15).
6. Run all cells in the notebook.
7. Two JSON files will be generated automatically:

   * One containing the **evaluation results**
   * One containing the **generated code**

---

### **2. DS1000 Dataset**

1. Open the `DS1000` folder.
2. Create **three API tokens**:

   * From **OpenRouter**, **OpenAI**, and **Hugging Face**.
3. Add your API keys in the first cell.
4. Optionally adjust the **"Number of Rows to Test"** (default = 15).
5. Run all cells.
6. Two JSON output files will be generated:

   * Results file
   * Generated code file

---

### **3. APPS Dataset**

1. Open the `APPS` folder.
2. Create **three API tokens**:

   * From **OpenRouter**, **OpenAI**, and **Hugging Face**.
3. Add your API keys in the first cell.
4. Adjust the **"Number of Rows to Test"** (default = 15).
5. Run all cells in the notebook.
6. Generated results and code will be saved as JSON files.

---

### **4. MBBP Dataset**

1. Open the `MBBP` folder.
2. Create **three API tokens**:

   * From **OpenRouter**, **OpenAI**, and **Hugging Face**.
3. Add your API keys in the first cell.
4. Modify the **"Number of Rows to Test"** value if needed (default = 15).
5. Run all notebook cells.
6. The results and generated code will be saved as JSON files.

---

## 📊 **Output**

Each notebook produces two output JSON files:

1. `results_<dataset>.json` — Model-wise evaluation results
2. `generated_code_<dataset>.json` — Generated code snippets or responses

These files can be used for further analysis, visualization, or report generation.

---

## 🧾 **Dependencies**

Make sure you have the following installed (Colab includes most by default):

```bash
!pip install openai datasets huggingface_hub
```

---

## 💡 **Notes**

* Default number of rows tested: **15** (you can increase this for broader evaluation).
* All notebooks are designed for **Google Colab** — no local setup required.
* Each run saves both **quantitative** and **qualitative** outputs for later comparison.

---

## 📈 **Future Improvements**

* Integration of evaluation metrics (BLEU, CodeBLEU, Pass@k)
* Aggregated performance dashboards
* Automated visual report generation

---

## 🧑‍💻 **Author**

Developed and maintained by **[Your Name]**

For research, analysis, and benchmarking of advanced LLM performance.

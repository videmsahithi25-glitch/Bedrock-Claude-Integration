# 📊 Prompt Evaluations with AWS Bedrock

A complete **prompt evaluation pipeline** using **AWS Bedrock** and **Claude Haiku**. Automatically generates test datasets, runs prompts, and grades outputs using both syntax validation and AI-based scoring.

---

## 📁 Files

```
├── 001_Prompt_Evals_complete.ipynb   # Main evaluation notebook
├── dataset.json                       # Auto-generated test dataset
└── README_PromptEvals.md             # This file
```

---

## 🧠 How It Works

```
Step 1 → Generate Dataset    (Claude creates test cases)
Step 2 → Run Prompt          (Claude solves each task)
Step 3 → Grade by Model      (Claude scores the solution)
Step 4 → Grade Syntax        (Python validates the format)
Step 5 → Final Score         (average of both scores)
```

---

## 📋 What the Pipeline Does

| Step | Function | Description |
|---|---|---|
| 1 | `generate_dataset()` | Generates 3 AWS-related tasks (Python / JSON / Regex) |
| 2 | `run_prompt()` | Sends each task to Claude to solve |
| 3 | `grade_by_model()` | Claude reviews and scores the solution 1-10 |
| 4 | `grade_syntax()` | Validates Python/JSON/Regex syntax automatically |
| 5 | `run_eval()` | Runs all cases and prints average score |

---

## ⚙️ Setup

### 1. Install dependencies
```bash
pip install boto3 jupyter notebook
```

### 2. Configure AWS credentials
```bash
aws configure
```

### 3. Run the notebook
```bash
jupyter notebook
```
Open `001_Prompt_Evals_complete.ipynb`

---

## 🌐 Model Used

```
us.anthropic.claude-3-5-haiku-20241022-v1:0
```
Claude Haiku is used for speed and cost efficiency during evaluations.

> ⚠️ Request model access in AWS Bedrock console before running

---

## 📊 Sample Output

```json
[
  {
    "task": "Validate an AWS S3 bucket name",
    "format": "regex",
    "score": 9.0,
    "reasoning": "Correctly enforces naming rules and length constraints"
  }
]
```

---

## 📝 License
MIT License

---

## 🙋 Author
**videmsahithi25-glitch** — Built with AWS Bedrock + Claude Haiku

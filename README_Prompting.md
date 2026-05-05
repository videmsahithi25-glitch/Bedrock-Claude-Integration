# 📊 Prompt Engineering & Evaluation with AWS Bedrock

An advanced **prompt evaluation framework** using **AWS Bedrock** and **Claude Sonnet**. Automatically generates test datasets, runs prompts concurrently, grades outputs using AI scoring, and produces a detailed **HTML report**.

---

## 📁 Files

```
├── 002_Prompting_Evaluation.ipynb   # Main evaluation notebook
├── dataset.json                      # Auto-generated test dataset
├── output.json                       # Evaluation results in JSON
├── output.html                       # Visual HTML evaluation report
└── README_Prompting.md              # This file
```

---

## 🧠 How It Works

```
Step 1 → Generate unique test ideas     (Claude brainstorms scenarios)
Step 2 → Generate test cases            (Claude creates inputs + criteria)
Step 3 → Run prompt on each test case   (Claude solves each task)
Step 4 → Grade each output              (Claude scores 1-10 with reasoning)
Step 5 → Generate HTML report           (Visual summary of all results)
```

---

## 🏗️ Key Components

| Component | Description |
|---|---|
| `PromptEvaluator` class | Full evaluation pipeline in one class |
| `generate_unique_ideas()` | Brainstorms diverse test scenarios |
| `generate_test_case()` | Creates inputs and solution criteria |
| `grade_output()` | AI-based scoring with strict rubric |
| `run_evaluation()` | Runs all cases concurrently + saves results |
| `generate_prompt_evaluation_report()` | Builds a styled HTML report |

---

## ⚡ Key Features

- ✅ **Concurrent execution** — runs multiple test cases simultaneously
- ✅ **AI grading** — Claude scores outputs 1-10 with reasoning
- ✅ **HTML report** — colour-coded scores (green/yellow/red)
- ✅ **JSON output** — machine-readable results
- ✅ **Strict scoring rubric** — mandatory criteria enforced

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
Open `002_Prompting_Evaluation.ipynb`

---

## 📊 Sample HTML Report Output

| Scenario | Score | Reasoning |
|---|---|---|
| Technical CS terminology | 9/10 | Meets all criteria |
| Medical research findings | 8/10 | Minor issues |
| Complex math concepts | 10/10 | Perfect match |

---

## 🌐 Model Used

```
us.anthropic.claude-3-5-sonnet-20241022-v2:0
```
Via AWS Bedrock in `us-west-2`

> ⚠️ Request model access in AWS Bedrock console before running

---

## 📝 License
MIT License

---

## 🙋 Author
**videmsahithi25-glitch** — Built with AWS Bedrock + Claude Sonnet

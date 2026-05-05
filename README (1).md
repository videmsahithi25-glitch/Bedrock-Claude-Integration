# 🚀 Amazon Bedrock + Claude Integration

Hands-on Jupyter Notebook projects using **AWS Bedrock** and **Anthropic Claude** models. Covers API requests, multi-turn conversations, system messages, vector databases, RAG pipelines, prompt caching, hybrid search, and prompt evaluation.

---

## 📁 Project Structure

```
├── 001_Api_Requests_complete.ipynb      # Basic API requests + chatbot
├── requirements.txt
├── .gitignore
└── README.md
```

---

## ⚙️ Setup & Installation

### 1. Clone the repository
```bash
git clone https://github.com/videmsahithi25-glitch/amazon-bedrock-integration.git
cd amazon-bedrock-integration
```

### 2. Create a virtual environment
```bash
python -m venv venv
source venv/bin/activate        # Mac/Linux
venv\Scripts\activate           # Windows
```

### 3. Install dependencies
```bash
pip install -r requirements.txt
```

### 4. Configure AWS credentials
```bash
aws configure
```
You will need:
- AWS Access Key ID
- AWS Secret Access Key
- Default region: `us-west-2`

> ⚠️ Never hardcode or commit your AWS credentials

### 5. Run the notebooks
```bash
jupyter notebook
```

---

## 📦 Requirements

```
boto3
jupyter
notebook
```

---

## 🧠 Topics Covered

| Notebook | Topic |
|---|---|
| 001 | API requests to Claude via Bedrock + multi-turn chatbot |

> More notebooks coming soon!

---

## 🌐 Model Used

```
us.anthropic.claude-sonnet-4-20250514-v1:0
```
Via AWS Bedrock in `us-west-2`

> ⚠️ You may need to request model access in the AWS Bedrock console before running

---

## 📝 License
MIT License

---

## 🙋 Author
**videmsahithi25-glitch** — Built with AWS Bedrock + Anthropic Claude

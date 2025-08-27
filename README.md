---

```markdown
# Advanced Shell Scripting – Pokémon API Automation

## 📌 Project Overview & Summary
This project is a **practical deep dive into Advanced Shell Scripting**, with a strong focus on **automating interactions with a RESTful API (Pokémon API)**.  
It progresses from **simple single API calls** to **complex automation tasks** involving:
- Parallel processing  
- Robust error handling  
- Retry logic  
- Data summarization  

The main goal is to **simulate real-world DevOps and Data Engineering tasks** where automation, reliability, and efficiency are critical.

---

## 🎯 Learning Objectives
By completing this project, you will gain hands-on proficiency in:

- **API Interaction** → Making HTTP requests with `curl`.
- **JSON Manipulation** → Parsing and extracting structured data using `jq`.
- **Text Processing** → Transforming outputs with `awk`, `sed`, and `grep`.
- **Robust Scripting** → Implementing error handling, retries, and logging.
- **Process Management** → Running tasks in parallel with background processes (`&`, `wait`, `$!`).
- **Data Reporting** → Generating reports in CSV format and computing averages with `awk`.
- **Modular Script Design** → Writing maintainable and reusable automation scripts.

---

## 🧩 Key Concepts
- **HTTP Status Codes** → Checking success/failure of requests (e.g., `200 OK` vs `404 Not Found`).
- **Idempotency & Retries** → Designing operations that can be safely retried after failures.
- **Rate Limiting** → Respecting API usage policies by adding delays between requests.
- **Concurrency vs Parallelism** → Using background jobs effectively while managing shared resources.
- **Data Pipelines (ETL)** → Automating the flow from extraction → transformation → loading → reporting.

---

## 🛠️ Tools & Libraries
- [`curl`](https://curl.se/) → Sending HTTP requests.
- [`jq`](https://stedolan.github.io/jq/) → JSON parsing and filtering.
- [`awk`](https://www.gnu.org/software/gawk/) → Data processing, aggregation, CSV generation.
- [`sed`](https://www.gnu.org/software/sed/) → Stream editing and text transformation.
- Core Shell Utilities: `grep`, `cut`, `echo`, loops, functions, conditionals, and job control (`&&`, `||`, `&`, `wait`).

---

## 🌍 Real-World Use Case
This project mirrors **ETL pipeline automation** in DevOps/Data Engineering:

1. **Extraction** → Fetch data from external APIs (Pokémon API simulates SaaS platforms like Twitter, Shopify, Salesforce).  
2. **Transformation** → Parse and clean JSON into structured formats (CSV).  
3. **Loading & Reporting** → Save processed data for BI tools (e.g., Tableau, Power BI).  

> The skills gained here are directly transferable to **building real ETL/ELT pipelines** in cloud and data workflows.

---

## 📂 Project Structure

```

ALXprodev-Devops/
│── Advanced\_shell/
│   ├── apiAutomation-0x00           # Task 0 – Single API Request
│   ├── data\_extraction\_automation-0x01 # Task 1 – Data Extraction
│   ├── batchProcessing-0x02         # Task 2 & 4 – Batch Processing with Error Handling
│   ├── summaryData-0x03             # Task 3 – Data Summarization & Reporting
│   ├── batchProcessing-0x04         # Task 5 – Parallel Processing
│   ├── errors.txt                   # Error logs
│   ├── pokemon\_data/                # Folder for JSON responses
│   └── pokemon\_report.csv           # Final CSV report

````

---

## 📜 Tasks Breakdown

### 0. API Request Automation
- Fetch data for **Pikachu** using `curl`.
- Save response to `data.json`.
- Log errors to `errors.txt`.

### 1. Extract Pokémon Data
- Parse JSON using `jq`, `awk`, `sed`.
- Output in human-readable format:  
  `"Pikachu is of type Electric, weighs 6kg, and is 0.4m tall."`

### 2. Batch Pokémon Data Retrieval
- Loop through multiple Pokémon `[Bulbasaur, Ivysaur, Venusaur, Charmander, Charmeleon]`.
- Save each response into a separate JSON file.
- Handle rate limiting with delays.

### 3. Summarize Pokémon Data
- Extract `name`, `height`, `weight` from JSON files.
- Generate a **CSV report** with averages (height & weight).

### 4. Error Handling & Retry Logic
- Implement retry mechanism (up to 3 attempts).
- Log failures to `errors.txt`.

### 5. Parallel Data Fetching
- Speed up data retrieval using **background jobs (`&`)**.
- Ensure proper process synchronization (`wait`).

---

## ✅ Project Assessment
Your project will be evaluated through:

- **Manual Review** → Code correctness, clarity, and functionality.
- **Auto-checks** → Ensuring required files exist.

⚠️ **Submit before the deadline** to generate your review link.

---

## 🚀 Getting Started

### 1. Clone Repository
```bash
git clone https://github.com/<your-username>/ALXprodev-Devops.git
cd ALXprodev-Devops/Advanced_shell
````

### 2. Make Scripts Executable

```bash
chmod +x apiAutomation-0x00 data_extraction_automation-0x01 batchProcessing-0x02 summaryData-0x03 batchProcessing-0x04
```

### 3. Run Scripts

```bash
./apiAutomation-0x00       # Fetch Pikachu data
./data_extraction_automation-0x01
./batchProcessing-0x02     # Batch fetch
./summaryData-0x03         # Generate report
./batchProcessing-0x04     # Parallel fetch
```

---

## ✨ Author

👤 **Chrispin Odiwuor**

* Software Engineering | DevOps | AWS Cloud Computing
* [LinkedIn](https://www.linkedin.com/) | [GitHub](https://github.com/)

---

```

---

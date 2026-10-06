# 🎓 AI Marks Analyzer

An AI-powered student marks analyzer that analyzes academic performance from student marks data and generates personalized insights and study recommendations using a locally running LLM.

## ✨ Features

* 📊 Calculates total marks and overall percentage
* 📈 Identifies strongest subjects
* 📉 Identifies subjects that need improvement
* 🏆 Finds the highest and lowest scoring subjects
* 🤖 Uses a local AI model to analyze student performance
* 💡 Generates study recommendations
* 🔒 Runs the AI model locally using Ollama

## 🛠️ Tech Stack

* **Python**
* **Pandas** — Data processing and analysis
* **NumPy** — Numerical operations
* **Ollama** — Local AI model interface
* **Qwen 2.5 Coder 3B** — Local LLM

## 📁 Project Structure

```text
ai-marks-analyzer/
│
├── data/
│   └── student_marks.csv
│
├── analyzer.py
│
└── README.md
```

## ⚙️ How It Works

The application follows a simple pipeline:

```text
Student Marks CSV
       ↓
   Pandas
       ↓
Calculate Performance
       ↓
Identify Strengths & Weaknesses
       ↓
Create AI Prompt
       ↓
Ollama + Qwen 2.5 Coder
       ↓
AI Performance Analysis
```

The program reads student information from the CSV file and calculates:

* Total marks
* Percentage
* Strong subjects
* Weak subjects
* Highest-scoring subject
* Lowest-scoring subject

These results are then passed to the local AI model, which generates an academic analysis containing:

1. Area needing improvement
2. Overall performance
3. Study recommendations

## 🚀 Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/Nimesh1205/ai-marks-analyzer.git
cd ai-marks-analyzer
```

### 2. Create a virtual environment

```bash
python -m venv .venv
```

Activate it on Windows:

```bash
.venv\Scripts\activate
```

### 3. Install dependencies

```bash
pip install numpy pandas ollama
```

### 4. Install Ollama

Install Ollama from its official website and make sure it is running on your system.

Then pull the model:

```bash
ollama pull qwen2.5-coder:3b
```

### 5. Run the analyzer

```bash
python analyzer.py
```

Enter the student's roll number when prompted.

## 🧪 Example

```text
Enter Student's Roll No:
101
```

The program first displays a marksheet containing the student's performance statistics and then sends the calculated results to the AI model.

The AI generates an analysis such as:

```text
1. Area Needing Improvement
   - Physics requires additional attention.

2. Overall Performance
   - The student is performing well overall.

3. Study Recommendations
   - Focus on weaker subjects.
   - Practice regularly.
   - Maintain strengths in high-scoring subjects.
```

## 🔮 Future Improvements

* [ ] Add a graphical user interface
* [ ] Add student performance charts
* [ ] Add grade calculation
* [ ] Add class-level performance comparison
* [ ] Generate downloadable reports
* [ ] Add subject-wise recommendations
* [ ] Add performance trends
* [ ] Add a web interface
* [ ] Improve error handling for invalid roll numbers
* [ ] Allow users to upload their own CSV files

## 🎯 Purpose

This project was built to explore how **Python data analysis and local AI models can be combined to create useful educational tools**.

It is also a learning project focused on working with:

* DataFrames
* CSV datasets
* Data analysis
* Prompt engineering
* Local LLMs
* Python libraries
* AI-assisted applications

## 📄 License

This project is intended for educational and learning purposes.

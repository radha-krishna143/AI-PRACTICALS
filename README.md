# Artificial Intelligence — Laboratory Practicals (5–12)

**Marwadi University | Department of Computer Science and Engineering (AI & ML)**

This repository contains the Jupyter Notebook submissions for **Artificial Intelligence (course code: `01AI0511`)**, covering **Practical 5 through Practical 12**. The experiments demonstrate foundational AI approaches to rule-based expert systems, constraint satisfaction, probabilistic inference, text classification, automated planning, sequential decision-making, logical inference, and machine learning.

> **Submission scope:** Only **Practicals 5–12** are included, as required for this submission. Practicals 1–4 are intentionally excluded.

## Student information

| Field | Details |
|---|---|
| **Student name** | **Hanmamolla Radha krishna** |
| **Enrollment number** | **92460118285** |
| **University** | **Marwadi University** |
| **Program / branch** | **Computer Science and Engineering (AI & ML)** |
| **Academic year of study** | **3rd Year** |
| **Semester** | **5th Semester** |
| **Section** | **5EN19** |
| **Subject** | **Artificial Intelligence** |
| **Course code** | **01AI0511** |
| **Course credits** | **4** |
| **Submission** | **AI Lab — Practicals 5 to 12** |

## Practical index

Each practical is an independent Python/Jupyter Notebook. The official practical objectives are listed in the [course syllabus](syllabus/Artificial_Intelligence_Course_Syllabus_01AI0511.pdf); the descriptions below identify what each uploaded notebook actually implements.

| Practical | Topic | Implementation / outcome | Notebook |
|:---:|---|---|---|
| **05** | Rule-Based Expert System | Uses IF–THEN rules for a laptop troubleshooting advisory system. | [Open Practical 05](practicals/Practical_05_Rule_Based_Expert_System.ipynb) |
| **06** | Constraint Satisfaction (CSP) | Solves map coloring with backtracking and neighbor-consistency checks. | [Open Practical 06](practicals/Practical_06_Map_Coloring_Backtracking.ipynb) |
| **07** | Probabilistic Reasoning | Trains a Bernoulli Naive Bayes model to predict `Flu` or `Cold` from symptoms, including class probabilities. | [Open Practical 07](practicals/Practical_07_Naive_Bayes_Diagnosis.ipynb) |
| **08** | Text Classification, Ethics & Explainability | Classifies messages as `Spam` or `Not Spam` using CountVectorizer and Multinomial Naive Bayes; discusses privacy, bias and explainability. | [Open Practical 08](practicals/Practical_08_Spam_Text_Classification.ipynb) |
| **09** | STRIPS / Goal-Stack Planning | Produces a simple robot-navigation plan using action preconditions and effects. | [Open Practical 09](practicals/Practical_09_STRIPS_Goal_Stack_Planning.ipynb) |
| **10** | Value Iteration | Finds state values and a policy in a small 2 × 2 grid-world. | [Open Practical 10](practicals/Practical_10_Grid_World_Value_Iteration.ipynb) |
| **11** | Propositional Logic & Inference | Derives conclusions in a weather-advisory example using logical rules and forward reasoning. | [Open Practical 11](practicals/Practical_11_Propositional_Logic_Inference.ipynb) |
| **12** | k-Nearest Neighbors (k-NN) | Predicts `Pass` or `Fail` from study data and compares predictions against expected labels. | [Open Practical 12](practicals/Practical_12_KNN_Student_Prediction.ipynb) |

## Repository structure

```text
Artificial-Intelligence-Lab-Practicals/
├── README.md
├── requirements.txt
├── .gitignore
├── practicals/
│   ├── Practical_05_Rule_Based_Expert_System.ipynb
│   ├── Practical_06_Map_Coloring_Backtracking.ipynb
│   ├── Practical_07_Naive_Bayes_Diagnosis.ipynb
│   ├── Practical_08_Spam_Text_Classification.ipynb
│   ├── Practical_09_STRIPS_Goal_Stack_Planning.ipynb
│   ├── Practical_10_Grid_World_Value_Iteration.ipynb
│   ├── Practical_11_Propositional_Logic_Inference.ipynb
│   └── Practical_12_KNN_Student_Prediction.ipynb
└── syllabus/
    └── Artificial_Intelligence_Course_Syllabus_01AI0511.pdf
```

## Prerequisites

- **Python 3.10+** and **pip**.
- JupyterLab (installed via `requirements.txt`).
- scikit-learn for Practicals **07, 08 and 12**; the other practicals rely on Python's standard library.
- A local Python environment is recommended. The notebooks use small examples and do not require external datasets, API keys, or internet access after installation.

## Setup and execution (Windows / PowerShell)

1. Download the repository from GitHub as a ZIP and extract it, or clone it with `git clone`. Open PowerShell inside the extracted `Artificial-Intelligence-Lab-Practicals` folder.
2. Create a virtual environment:

   ```powershell
   py -m venv .venv
   ```

3. Activate it:

   ```powershell
   .\.venv\Scripts\Activate.ps1
   ```

   If your PowerShell policy prevents activation, skip this step and use `.\.venv\Scripts\python.exe` in place of `python` in the commands below.

4. Install the required packages:

   ```powershell
   python -m pip install --upgrade pip
   python -m pip install -r requirements.txt
   ```

5. Launch JupyterLab:

   ```powershell
   python -m jupyter lab
   ```

6. In JupyterLab, open `practicals/`, select a notebook, and execute its code cells from top to bottom using **Shift + Enter** (or **Run → Run All Cells**). Save it after running if your instructor requires executed outputs.

**Notes:** Practicals **05** and **08** contain interactive `input()` prompts. Enter responses when requested. Results may vary if you change example data. No separate data files are needed.

## Alternative: Google Colab

Open [Google Colab](https://colab.research.google.com/), choose **Upload**, and upload an `.ipynb` file from the `practicals` folder. Run the cells in order. Colab typically provides scikit-learn, but install it in a notebook cell (`%pip install scikit-learn`) if your environment requires it.

## Publish as a GitHub repository

1. Sign in to GitHub and create a **new, empty repository**, for example `Artificial-Intelligence-Lab-Practicals`. Do not initialize it with a separate README if you plan to follow the commands below.
2. Open PowerShell in the repository root folder (the folder containing this README).
3. Run:

   ```powershell
   git init
   git add .
   git commit -m "Add Artificial Intelligence practicals 5-12"
   git branch -M main
   git remote add origin https://github.com/YOUR_USERNAME/Artificial-Intelligence-Lab-Practicals.git
   git push -u origin main
   ```

   Replace **`YOUR_USERNAME`** with your own GitHub username. Git must be installed and GitHub authentication must be configured. If Git asks for your identity, set `git config --global user.name "Your Name"` and `git config --global user.email "you@example.com"` using the email associated with your Git commits.

**No terminal needed?** On the empty repository page, choose **uploading an existing file**, then upload the contents of this folder (including `README.md`, `requirements.txt`, `.gitignore`, `practicals/`, and `syllabus/`) and commit. GitHub does not automatically unpack an uploaded ZIP into repository files, so **extract the ZIP first**.

## Lab submission checklist

- [ ] Only Practicals **05–12** appear under `practicals/`.
- [ ] Each notebook opens successfully in Jupyter or Colab.
- [ ] Required dependencies are installed before running Practicals 07, 08 and 12.
- [ ] Code cells are executed in order, including answers to interactive prompts in Practicals 05 and 08.
- [ ] Outputs and conclusions are checked, and notebooks are saved if execution evidence is expected.
- [ ] Student name, enrollment number, semester, branch, and section match college records.
- [ ] The GitHub repository contains **individual notebook files**, not only a ZIP archive.
- [ ] The final repository URL is shared with the instructor or submitted through the requested platform.

## Academic reference

The included syllabus is for **Artificial Intelligence (`01AI0511`)** at **Marwadi University**. It lists the suggested experiments, including Practicals 5–12 on page 3. This repository uses the supplied notebooks as-is; it does not claim that the notebooks or generated outputs were independently re-executed or instructor-approved.

---

**Prepared for academic practical submission by Hanmamolla Radha krishna — Enrollment No. 92460118285 — Section 5EN19.**

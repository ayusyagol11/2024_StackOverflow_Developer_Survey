# 📊 2024 Stack Overflow Developer Survey Analysis  
**Unlocking Insights into AI Adoption, Salary Trends, and Developer Productivity**  
[![Python](https://img.shields.io/badge/Python-3.10%2B-blue)](https://python.org)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange)](https://jupyter.org)
[![Plotly](https://img.shields.io/badge/Visualization-Plotly-green)](https://plotly.com)

Welcome to the 2024 Stack Overflow Developer Survey Analysis! In this project, we explore developer trends, technology adoption, AI integration, and job satisfaction using insights from over 65,000 developers worldwide.

Through data cleaning, exploratory analysis, and visualization, we uncover key insights into how developers work, learn, and interact with AI & Stack Overflow.


⸻

📖 Table of Contents

1️⃣ Introduction
2️⃣ Dataset Overview
3️⃣ Data Cleaning & Preprocessing
4️⃣ Exploratory Data Analysis (EDA)
5️⃣ Answering Key Questions
6️⃣ Conclusion & Insights
7️⃣ How to Use This Project

⸻

📝 Introduction

Why This Project?
The Stack Overflow Developer Survey is one of the largest and most comprehensive datasets on software development. By analyzing this dataset, we can:
✅ Identify the most popular programming languages & tools.
✅ Understand how AI is shaping developer workflows.
✅ Explore salary trends & job satisfaction.
✅ Identify developer frustrations & challenges.

⸻

📊 Dataset Overview

📥 Data Source:

🔗 The dataset was downloaded from Stack Overflow’s Official Survey

📂 Structure of the Dataset:
	•	65,437 responses from developers worldwide 🌍
	•	114 columns covering:
	•	🌐 Programming languages, frameworks, and tools
	•	🤖 AI adoption & trust in AI-generated code
	•	💰 Salaries & job satisfaction
	•	🚀 Learning resources & Stack Overflow usage

⸻

🛠️ Data Cleaning & Preprocessing

🔎 Steps Taken:

1️⃣ Checked for Missing Values
	•	Many columns had high missing values (e.g., AINextMuch less integrated, EmbeddedAdmired).
	•	Dropped columns with >50% missing data.
	•	Filled missing categorical values with "Unknown".
	•	Filled missing numerical values with median values.

2️⃣ Checked for Duplicates
	•	Removed all duplicate rows to avoid redundancy.

3️⃣ Fixed Data Types
	•	Converted salary & experience fields to numeric values.
	•	Standardized categorical values (e.g., "Yes", "yes", "YES" → "yes").

4️⃣ Ensured Data Consistency
	•	Fixed multi-select fields (e.g., split languages & tools into separate counts).

⸻

📈 Exploratory Data Analysis (EDA)

1️⃣ Developer Demographics

📌 Age Distribution
	•	Most developers are aged 18-34 years.
	•	Fewer older developers, showing a younger workforce in tech.

📊 Education Level
	•	Majority hold a Bachelor’s or Master’s degree 🎓
	•	Some self-taught developers & bootcamp graduates.

plt.figure(figsize=(10, 5))
sns.countplot(data=df, y="Age", order=df["Age"].value_counts().index, hue="Age", legend=False, palette="coolwarm")
plt.title("Age Distribution of Developers")
plt.show()



⸻

2️⃣ Popular Programming Languages & Frameworks

📌 Most Used Languages
	•	Python, JavaScript, and SQL remain the top languages.
	•	Rust, Go, and TypeScript are gaining popularity.

📌 Most Wanted Languages
	•	Developers want to learn Rust, TypeScript, and Go.

plt.figure(figsize=(12, 5))
sns.barplot(data=used_languages.head(10), x="Count", y="Language", hue="Language", legend=False, palette="viridis")
plt.title("Top 10 Most Used Programming Languages")
plt.show()



⸻

3️⃣ AI Usage & Trust in AI

📌 AI Integration in Development
	•	75% of developers use AI-powered tools (ChatGPT, Copilot).
	•	Trust in AI varies—some rely on AI, others are skeptical.
	•	Some developers worry AI will replace jobs 🤖💼

plt.figure(figsize=(8, 4))
sns.countplot(data=df, y="AISelect", hue="AISelect", order=df["AISelect"].value_counts().index, legend=False, palette="coolwarm")
plt.title("Developers Using AI in Their Workflow")
plt.show()



⸻

4️⃣ Developer Frustrations & Productivity Challenges

📌 Top Challenges Faced
	•	“Poor documentation”, “tight deadlines”, “legacy code” are common frustrations.
	•	Many developers spend 30-60 mins daily searching for solutions.

📊 Word Cloud of Developer Frustrations

wordcloud = WordCloud(width=800, height=400, background_color="white", colormap="coolwarm").generate(" ".join(df["Frustration"].dropna()))
plt.imshow(wordcloud, interpolation="bilinear")
plt.axis("off")
plt.title("Biggest Developer Frustrations")
plt.show()



⸻

5️⃣ Stack Overflow Usage & Learning Trends

📌 How Developers Learn?
	•	Most rely on Stack Overflow, online courses, and documentation 📚
	•	AI-powered learning tools are growing in adoption.

📌 How Often Do Developers Visit Stack Overflow?
	•	50% visit daily or multiple times per day.
	•	Some rely on private documentation instead.

plt.figure(figsize=(10, 5))
sns.countplot(data=df, y="SOVisitFreq", hue="SOVisitFreq", order=df["SOVisitFreq"].value_counts().index, legend=False, palette="Blues_r")
plt.title("How Often Do Developers Visit Stack Overflow?")
plt.show()



⸻

💡 Conclusion & Insights

✅ AI is transforming development but trust in AI remains mixed.
✅ Python, JavaScript, and SQL remain dominant, but Rust & TypeScript are the future.
✅ Salaries increase with experience but plateau after 20+ years.
✅ Developers face major challenges with tight deadlines & outdated code.
✅ Stack Overflow & online courses are still essential learning resources.

⸻

📌 How to Use This Project?

💻 Requirements
	•	Python
	•	Jupyter Notebook
	•	Libraries: pandas, seaborn, matplotlib, wordcloud

📜 Run the Notebook:
	1.	Clone this repository
	2.	Install required libraries (pip install pandas seaborn matplotlib wordcloud)
	3.	Run jupyter notebook and open the .ipynb file
	4.	Execute the cells to see the analysis

⸻

🎯 Next Steps

🔹 Perform machine learning predictions (salary prediction, clustering).
🔹 Use Natural Language Processing (NLP) for sentiment analysis on developer frustrations.
🔹 Compare 2024 data with previous years to identify trends.

⸻

🔥 Thank you for exploring this project! Let me know if you have any suggestions or improvements! 🚀


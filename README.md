# 📊 2024 Stack Overflow Developer Survey Analysis  
**Unlocking Insights into AI Adoption, Salary Trends, and Developer Productivity**  
[![Python](https://img.shields.io/badge/Python-3.10%2B-blue)](https://python.org)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange)](https://jupyter.org)
[![Plotly](https://img.shields.io/badge/Visualization-Plotly-green)](https://plotly.com)
[![Matplotlib](https://img.shields.io/badge/Visualization-Matplotlib-green)](https://matplotlib.org/)

Welcome to the **2024 Stack Overflow Developer Survey Analysis!** In this project, I explore **developer trends, technology adoption, AI integration, and job satisfaction** using insights from over **65,000 developers worldwide**.  

Through **data cleaning, exploratory analysis, and visualization**, I uncover key insights into how developers work, learn, and interact with AI & Stack Overflow.  

---

## **📝 Introduction**  

### **Why This Project?**  
The **Stack Overflow Developer Survey** is one of the **largest** and **most comprehensive** datasets on software development. By analysing this dataset, we can:  
✅ Identify the **most popular programming languages** & tools.  
✅ Understand how **AI is shaping developer workflows**.  
✅ Explore **salary trends & job satisfaction**.  
✅ Identify **developer frustrations & challenges**.  

---

## **📊 Dataset Overview**  

### **📥 Data Source:**  
🔗 The dataset was downloaded from **[Stack Overflow's Official Survey](https://survey.stackoverflow.co/)**  

### **📂 Structure of the Dataset:**  
- **65,437 responses** from developers worldwide 🌍  
- **114 columns** covering:  
  - 🌐 **Programming languages, frameworks, and tools**  
  - 🤖 **AI adoption & trust in AI-generated code**  
  - 💰 **Salaries & job satisfaction**  
  - 🚀 **Learning resources & Stack Overflow usage**  

---

## **🛠️ Data Cleaning & Preprocessing**  

### **🔎 Steps Taken:**  
1️⃣ **Checked for Missing Values**  
   - Many columns had **high missing values** (e.g., `AINextMuch less integrated`, `EmbeddedAdmired`).  
   - **Dropped columns** with **>50% missing data**.  
   - **Filled missing categorical values** with `"Unknown"`.  
   - **Filled missing numerical values** with **median values**.  

2️⃣ **Checked for Duplicates**  
   - **Removed all duplicate rows** to avoid redundancy.  

3️⃣ **Fixed Data Types**  
   - Converted **salary & experience** fields to **numeric values**.  
   - Standardized categorical values (e.g., `"Yes"`, `"yes"`, `"YES"` → `"yes"`).  

4️⃣ **Ensured Data Consistency**  
   - Fixed multi-select fields (e.g., **split languages & tools** into separate counts).  

---

## **📈 Exploratory Data Analysis (EDA)**  

### **1️⃣ Developer Demographics**  
📌 **Age Distribution**

![Age Distribution of Developers](https://github.com/ayusyagol11/2024_StackOverflow_Developer_Survey/blob/main/chart_images/Age%20Distribution%20of%20Developers.png)
- Most developers are aged **18-34 years**.  
- **For older developers**, showing **a younger workforce in tech**.  

📌 **Education Level** 

![Education Level Distribution of Developers](https://github.com/ayusyagol11/2024_StackOverflow_Developer_Survey/blob/main/chart_images/Education%20Level%20Distribution%20of%20Developers.png)
- Majority hold a **Bachelor’s or Master’s degree** 🎓  
- Some **self-taught** developers & bootcamp graduates.  

---

### **2️⃣ Popular Programming Languages & Frameworks**  
📌 **Most Used Languages**  

![Top 10 Most Used Programming Languages](https://github.com/ayusyagol11/2024_StackOverflow_Developer_Survey/blob/main/chart_images/Top%2010%20Most%20Used%20Programming%20Languages.png)
- **Python, JavaScript, and SQL** remain the top languages.  
- **Rust, Go, and TypeScript** are gaining popularity.  

📌 **Most Wanted Languages**  

![Top 10 Most Desired Programming Languages](https://github.com/ayusyagol11/2024_StackOverflow_Developer_Survey/blob/main/chart_images/Top%2010%20Most%20Desired%20Programming%20Languages.png)
- Developers want to learn **Rust, TypeScript, and Go**.  

---

### **3️⃣ AI Usage & Trust in AI**  
📌 **AI Integration in Development**  

![Developers using AI in their workflow](https://github.com/ayusyagol11/2024_StackOverflow_Developer_Survey/blob/main/chart_images/developers-using-AI-in-their-workflow.png)
- **75% of developers** use **AI-powred tools** (ChatGPT, Copilot).  
- **Trust in AI varies**—some rely on AI, others are skeptical.  
- Some developers worry AI will **replace jobs** 🤖💼  

---

### **4️⃣ Developer Frustrations & Productivity Challenges**  
📌 **Top Challenges Faced**  

![Challenges developers face](https://github.com/ayusyagol11/2024_StackOverflow_Developer_Survey/blob/main/chart_images/Biggest%20Challenges%20Developers%20Face%20in%20the%20Workplace.png)
- **"Poor documentation", "tight deadlines", "legacy code"** are common frustrations.  
- Many developers spend **30-60 mins daily** searching for solutions.  

📊 **Word Cloud of Developer Frustrations**  


---

### **5️⃣ Stack Overflow Usage & Learning Trends**

📌 **How Developers Learn?**

![Top Learning methods among developers](https://github.com/ayusyagol11/2024_StackOverflow_Developer_Survey/blob/main/chart_images/top-learning-methods-among-developers.png)
- Most rely on Stack Overflow, online courses, and documentation 📚
- AI-powered learning tools are growing in adoption.

📌 **How Often Do Developers Visit Stack Overflow?**

![How often developers visit stack overflow](https://github.com/ayusyagol11/2024_StackOverflow_Developer_Survey/blob/main/chart_images/how-oftern-do-developers-visit-stack-overflow.png)
- 50% visit daily or multiple times per day.
- Some rely on private documentation instead.

---

### **💡 Conclusion & Insights**

- AI is transforming development, but trust in AI remains mixed.
- Python, JavaScript, and SQL remain dominant, but Rust & TypeScript are the future.
- Salaries increase with experience but plateau after 20+ years.
- Developers face major challenges with tight deadlines & outdated code.
- Stack Overflow & online courses are still essential learning resources.

---

### **📌 How to Use This Project?**

**💻 Requirements**
- Python
- Jupyter Notebook
- Libraries: pandas, seaborn, matplotlib, wordcloud

**📜 Run the Notebook:**
1. Clone this repository
2. Install required libraries (pip install pandas seaborn matplotlib wordcloud)
3. Run jupyter notebook and open the .ipynb file
4. Execute the cells to see the analysis

---

### **🎯 Next Steps**

🔹 Perform machine learning predictions (salary prediction, clustering).

🔹 Use Natural Language Processing (NLP) for sentiment analysis on developer frustrations.

🔹 Compare 2024 data with previous years to identify trends.

---

🔥 Thank you for exploring this project! Let me know if you have any suggestions or improvements! 🚀

---

Created by **Aayush Yagol**
[![LinkedIn](https://img.shields.io/badge/LinkedIn-blue)](https://www.linkedin.com/in/aayush-yagol-046874145/)
[![Porfolio](https://img.shields.io/badge/Portfolio-Black)](https://www.aayushyagol.com)

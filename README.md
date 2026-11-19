# Python & Visual Studio Code Setup Guide for macOS

**A beginner-friendly guide to installing Python, Visual Studio Code, extensions, and essential Python packages on macOS.**



---

## 📌 Table of Contents

1. [Introduction](#-introduction)
2. [What You Need](#-what-you-need)
3. [Step 1: Check Your Mac Processor](#-step-1-check-your-mac-processor)
4. [Step 2: Install Visual Studio Code](#-step-2-install-visual-studio-code)
5. [Step 3: Install Python](#-step-3-install-python)
6. [Step 4: Install VS Code Extensions](#-step-4-install-vs-code-extensions)
7. [Step 5: Configure Python in VS Code](#-step-5-configure-python-in-vs-code)
8. [Step 6: Create Your First Python Project](#-step-6-create-your-first-python-project)
9. [Step 7: Create a Virtual Environment](#-step-7-create-a-virtual-environment)
10. [Step 8: Install Python Packages](#-step-8-install-python-packages)
11. [Step 9: Test Your Installation](#-step-9-test-your-installation)
12. [Step 10: Save Package Requirements](#-step-10-save-package-requirements)
13. [Common Problems and Solutions](#-common-problems-and-solutions)
14. [Useful Resources](#-useful-resources)

---

## 🐍 Introduction

This guide explains how to set up a Python development environment on macOS using Visual Studio Code (VS Code).

It is designed for beginners who want to learn Python programming, data analytics, data science, automation, and machine learning.

By following this guide, you will learn how to:

- Install Visual Studio Code.
- Install Python on macOS.
- Configure Python inside VS Code.
- Install useful VS Code extensions.
- Create and activate virtual environments.
- Install essential Python packages.
- Run Python scripts and Jupyter notebooks.
- Organize and manage Python projects.

**What you will have at the end:**

A working Python development environment ready for programming and data analytics projects.

## 💻 What You Need

Before starting, make sure you have:

- A Mac running macOS.
- An internet connection.
- Permission to install applications.
- Basic knowledge of using your Mac.

You do not need previous Python programming experience.

## 🔹 Step 1: Check Your Mac Processor

First, identify which processor your Mac uses.

1. Click the Apple logo () in the top-left corner.
2. Select **About This Mac**.
3. Check the processor or chip information.

You should see one of the following:

| Processor | Version to Download |
|---|---|
| Apple M1, M2, M3, M4 or M5 | Apple Silicon |
| Intel processor | Intel |

You will need this information when downloading VS Code.

## 🔹 Step 2: Install Visual Studio Code

Visual Studio Code is a free code editor used to write, edit, and run Python programs.

### Download VS Code

1. Visit the official website:

   https://code.visualstudio.com/

2. Click **Download for Mac**.
3. Select the correct version for your processor.
4. Wait for the download to finish.

### Install VS Code

1. Open your Downloads folder.
2. Double-click the downloaded ZIP file.
3. Locate `Visual Studio Code.app`.
4. Drag the application into your Applications folder.
5. Open Applications.
6. Launch Visual Studio Code.

If macOS asks for confirmation, select Open.

**Installation complete!**

## 🔹 Step 3: Install Python

Python is the programming language we will use to develop applications, analyze data, and build projects.

### Download Python

1. Visit the official Python website:

   https://www.python.org/downloads/macos/

2. Download the latest stable Python 3 release.
3. Open the downloaded `.pkg` installer.
4. Follow the installation instructions.
5. Complete the installation.

### Verify Python Installation

Now we need to confirm that Python was installed correctly.

**Open Terminal:**

1. Press `Command + Space`.
2. Type `Terminal`.
3. Press Enter.

Enter this command:

```bash
python3 --version
```

You should see a Python version, for example:

```text
Python 3.x.x
```

Next, check whether pip is installed:

```bash
python3 -m pip --version
```

Pip is the package installer used to download and install Python libraries.

If both commands display version information, Python is ready.

## 🔹 Step 4: Install VS Code Extensions

Extensions add additional features to Visual Studio Code.

### How to Install Extensions

1. Open Visual Studio Code.
2. Click the Extensions icon on the left sidebar.
3. Alternatively, press:

   `Command + Shift + X`

4. Search for each extension below.
5. Click Install.

### Recommended Extensions

| Extension | Publisher | Purpose |
|---|---|---|
| Python | Microsoft | Python support |
| Pylance | Microsoft | Code suggestions and error detection |
| Jupyter | Microsoft | Create and run notebooks |
| Python Debugger | Microsoft | Find and fix errors |
| Python Environments | Microsoft | Manage Python environments |

**Important:** Install the official extensions published by Microsoft.

## 🔹 Step 5: Configure Python in VS Code

Now we need to connect the Python installation to VS Code.

1. Open VS Code.
2. Press `Command + Shift + P`.
3. Search for:

```text
Python: Select Interpreter
```

4. Select the Python 3 version you installed.

### Open the VS Code Terminal

Go to:

**Terminal → New Terminal**

Alternatively, use:

`Control + Backtick`

Enter:

```bash
python3 --version
```

If the Python version appears, the terminal can access Python.

## 🔹 Step 6: Create Your First Python Project

Let's create a folder where you can store your Python projects.

### Create a Project Folder

1. Open Finder.
2. Go to Documents.
3. Create a new folder called:

```text
Python-Projects
```

4. Open VS Code.
5. Select **File → Open Folder**.
6. Select the `Python-Projects` folder.

Your project folder should now appear in the VS Code Explorer panel.

### Create Your First Python File

1. Right-click inside the Explorer panel.
2. Select New File.
3. Name the file:

```text
hello.py
```

4. Add the following code:

```python
print("Hello, World!")
print("Welcome to Python programming!")
```

Save the file.

You have now created your first Python program.

## 🔹 Step 7: Create a Python Virtual Environment

A virtual environment allows you to install packages separately for each project.

This prevents package conflicts and keeps your projects organized.

### Create the Environment

Open the VS Code terminal and run:

```bash
python3 -m venv .venv
```

This creates a folder called `.venv` inside your project.

### Activate the Environment

Run:

```bash
source .venv/bin/activate
```

You should see something similar to:

```text
(.venv)
```

at the beginning of your terminal prompt.

This means your virtual environment is active.

### Upgrade pip

Run:

```bash
python -m pip install --upgrade pip
```

**Important:** Activate your virtual environment whenever you start working on this project.

To deactivate it:

```bash
deactivate
```

## 🔹 Step 8: Install Essential Python Packages

Python packages provide additional tools and functions that make programming easier.

For data analytics, I recommend starting with the following packages.

### 1. Data Analysis Packages

| Package | Description |
|---|---|
| pandas | Data cleaning, manipulation, and analysis |
| numpy | Numerical calculations and arrays |
| scipy | Scientific and mathematical calculations |
| statsmodels | Statistical analysis and modelling |

### 2. Data Visualization Packages

| Package | Description |
|---|---|
| matplotlib | Create charts and graphs |
| seaborn | Statistical data visualization |
| plotly | Create interactive charts and visualizations |

### 3. Excel and Database Packages

| Package | Description |
|---|---|
| openpyxl | Read and write Excel files |
| sqlalchemy | Connect Python to databases |
| pymysql | Connect Python to MySQL databases |
| pyodbc | Connect Python to databases using ODBC |

### 4. Machine Learning Packages

| Package | Description |
|---|---|
| scikit-learn | Machine learning algorithms |
| xgboost | Gradient boosting models |
| joblib | Save and load machine learning models |

### 5. Jupyter and Development Packages

| Package | Description |
|---|---|
| jupyter | Interactive Python notebooks |
| ipykernel | Python notebook kernel |
| requests | Retrieve information from APIs |
| beautifulsoup4 | Extract information from websites |

### Install All Essential Packages

Make sure your virtual environment is activated.

Copy and paste the following command into your VS Code terminal:

```bash
python -m pip install pandas numpy scipy statsmodels matplotlib seaborn plotly openpyxl sqlalchemy pymysql pyodbc scikit-learn xgboost joblib jupyter ipykernel requests beautifulsoup4
```

Press Enter and wait for the installation to finish.

**Note:** `pyodbc` may require additional system-level ODBC dependencies. You can skip it if you are not working with databases that require ODBC.

### Verify Package Installation

Run:

```bash
python -m pip list
```

This displays the packages installed in your environment.

## 🔹 Step 9: Test Your Python Installation

Let's test whether Python and the packages are working correctly.

### Create a Test File

Create a new Python file:

```text
test_python.py
```

Copy and paste this code:

```python
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns
import sklearn
import plotly

print("Python is working successfully!")

print("Pandas:", pd.__version__)
print("NumPy:", np.__version__)
print("Scikit-learn:", sklearn.__version__)
print("Plotly:", plotly.__version__)

print("All tests completed!")
```

Save the file.

### Run Your Python File

1. Make sure your `.venv` environment is active.
2. Open `test_python.py`.
3. Click the Run Python File button in the top-right corner.

Alternatively, run:

```bash
python test_python.py
```

If the program runs without errors, your installation is successful.

## 🔹 Step 10: Create Your First Data Analytics Project

Now let's use Python to perform a simple sales analysis.

Create a new file:

```text
sales_analysis.py
```

Copy the following code:

```python
import pandas as pd
import matplotlib.pyplot as plt

# Create sample sales data
data = {
    "Product": ["Laptop", "Phone", "Tablet", "Monitor"],
    "Sales": [5000, 3500, 2000, 1500],
    "Quantity": [5, 7, 4, 3]
}

# Create a DataFrame
df = pd.DataFrame(data)

# Calculate total sales
df["Total Sales"] = df["Sales"] * df["Quantity"]

# Display the dataset
print(df)

# Calculate total revenue
total_revenue = df["Total Sales"].sum()

print("Total Revenue:", total_revenue)

# Create a sales chart
df.plot(
    x="Product",
    y="Total Sales",
    kind="bar",
    title="Sales Performance"
)

plt.xlabel("Product")
plt.ylabel("Total Sales")
plt.tight_layout()
plt.show()
```

Run the file:

```bash
python sales_analysis.py
```

You should see the sales dataset, total revenue, and a bar chart.

Congratulations! You have completed your first Python data analysis exercise.

## 🔹 Step 11: Save Your Package Requirements

It is good practice to save the packages and their versions used in your project.

Run:

```bash
python -m pip freeze > requirements.txt
```

This creates a `requirements.txt` file.

When you want to recreate the environment in another project or computer, run:

```bash
python -m pip install -r requirements.txt
```

This installs the package versions listed in the requirements file.

## 📁 Recommended Project Structure

Organize your Python projects using a structure like this:

```text
Python-Projects/
│
├── Data-Analysis-Project/
│   │
│   ├── .venv/
│   ├── data/
│   ├── notebooks/
│   ├── scripts/
│   ├── outputs/
│   │
│   ├── requirements.txt
│   └── README.md
│
├── Python-Basics/
│   │
│   ├── hello.py
│   ├── variables.py
│   └── functions.py
│
└── Machine-Learning-Project/
```

**Important:** Do not upload your `.venv` folder to GitHub. It can be recreated using your `requirements.txt` file.

## 🛠️ Common Problems and Solutions

### Problem 1: Python command not found

Try:

```bash
python3 --version
```

If Python is still not found, check whether the Python installer completed successfully.

### Problem 2: Pip is not working

Try:

```bash
python3 -m ensurepip --upgrade
```

Then:

```bash
python3 -m pip --version
```

### Problem 3: VS Code cannot find Python

1. Press `Command + Shift + P`.
2. Search for `Python: Select Interpreter`.
3. Select your installed Python interpreter or project `.venv` interpreter.

### Problem 4: Permission denied when installing packages

Do not use `sudo pip install`.

First, activate your virtual environment:

```bash
source .venv/bin/activate
```

Then install the package:

```bash
python -m pip install package_name
```

### Problem 5: Virtual environment is not activating

Make sure you are inside the correct project folder.

Run:

```bash
source .venv/bin/activate
```

If `.venv` does not exist, recreate it:

```bash
python3 -m venv .venv
```

## 📚 Useful Learning Resources

| Resource | Description |
|---|---|
| [Python Official Website](https://www.python.org/) | Download Python |
| [Python Documentation](https://docs.python.org/3/) | Official Python documentation |
| [VS Code](https://code.visualstudio.com/) | Download Visual Studio Code |
| [Pandas Documentation](https://pandas.pydata.org/docs/) | Learn data analysis |
| [NumPy Documentation](https://numpy.org/doc/) | Learn numerical computing |
| [Matplotlib Documentation](https://matplotlib.org/stable/) | Learn data visualization |
| [Scikit-learn Documentation](https://scikit-learn.org/stable/) | Learn machine learning |
| [Jupyter Documentation](https://docs.jupyter.org/) | Learn Python notebooks |

---

## ✅ Final Installation Checklist

Before starting your Python journey, make sure you have completed these steps:

- [ ] Installed Visual Studio Code.
- [ ] Installed Python 3.
- [ ] Installed Python extensions.
- [ ] Configured the Python interpreter.
- [ ] Created a Python project folder.
- [ ] Created a virtual environment.
- [ ] Installed essential Python packages.
- [ ] Successfully ran `test_python.py`.
- [ ] Successfully completed the sales analysis exercise.
- [ ] Created a `requirements.txt` file.

## 🎯 What's Next?

After completing this setup, I recommend learning Python in the following order:

1. **Python Fundamentals:** Variables, data types, operators, loops, conditions, and functions.
2. **Data Structures:** Lists, tuples, dictionaries, and sets.
3. **NumPy:** Arrays and numerical operations.
4. **Pandas:** Data cleaning, manipulation, and analysis.
5. **Matplotlib & Seaborn:** Data visualization.
6. **SQL with Python:** Database connections and querying.
7. **Exploratory Data Analysis (EDA):** Working with real-world datasets.
8. **Machine Learning:** Introduction to predictive modelling.

---

**Author:** Daniel Sowah

**Focus:** Data Analytics | Business Intelligence | Python | SQL | Data Science

*This guide is created for beginners who want to set up Python on macOS and start learning programming and data analytics.*

If you find this guide useful, feel free to ⭐ star the repository and share it with others who are learning Python.

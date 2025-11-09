<<<<<<< HEAD
# 🧮 Dynamic Storage Allocation Simulator

**Name:** Sowjanya Teppali  
**Student ID:** 11857046  
**Assignment:** ICE - Dynamic Storage Allocation (First Fit, Best Fit, Worst Fit)

---

## 🎯 Objective

To simulate **dynamic memory allocation strategies** used in Operating Systems —  
namely **First Fit**, **Best Fit**, and **Worst Fit**-and compare their performance in terms of **internal fragmentation**.

---

## 📝 Description

The program accepts:
- The number and sizes of memory blocks
- The number and sizes of processes
It then assigns each process to memory blocks according to the chosen allocation strategies:
1. **First Fit:** Assigns the first block large enough for the process.
2. **Best Fit:** Assigns the smallest block large enough for the process.
3. **Worst Fit:** Assigns the largest available block.

After allocation, the program displays:
- Which process was assigned to which memory block
- The overall **internal fragmentation** for each approach
This version replicates the **textbook sample output for conceptual understanding.
---

## ⚙️ Parameter Passing

- Memory blocks and their sizes are kept in Python lists
- Memory blocks and process sizes are stored in **Python lists**.
- Lists are passed as parameters to each allocation function:
  - `first_fit(blocks, processes)`
  - `best_fit(blocks, processes)`
  - `worst_fit(blocks, processes)`
- Each function returns:
  - A list, known as an **allocation list**, displaying the block assignments
  - The total **internal fragmentation** value.

---

## 💻 Sample Input & Output

### **Input:**
Enter number of memory blocks: 5
Enter block sizes: 100 500 200 300 600
Enter number of processes: 4
Enter process sizes: 212 417 112 426

### **Output:**
First Fit:
Process 1 -> Block 3
Process 2 -> Block 5
Process 3 -> Block 1
Process 4 -> Block 5

Internal Fragmentation (First Fit): 357

Best Fit:
Process 1 -> Block 4
Process 2 -> Block 5
Process 3 -> Block 1
Process 4 -> Block 2

Internal Fragmentation (Best Fit): 339

Worst Fit:
Process 1 -> Block 5
Process 2 -> Block 5
Process 3 -> Block 4
Process 4 -> Block 2

Internal Fragmentation (Worst Fit): 401

---

## 📘 Explanation

| Strategy  | Approach | Description |
|------------|-----------|--------------|
| **First Fit** | Sequential search | Allocates to the first block large enough for the process. |
| **Best Fit** | Optimal block selection | Finds the smallest block that still fits the process. |
| **Worst Fit** | Largest block selection | Chooses the block with the most remaining space. |

- **Internal Fragmentation** is the total unused space within allocated blocks.
- The simulation highlights the efficiency differences between allocation strategies.

---

## 🧩 Files Included

| File Name | Description |
|------------|--------------|
| `dynamic_allocation.py` | Python source code for allocation strategies |
| `README.md` | Project documentation |

---

## ✅ Result Summary

| Strategy | Total Internal Fragmentation |
|-----------|------------------------------|
| First Fit | 357 |
| Best Fit  | 339 |
| Worst Fit | 401 |

---

**End of Report**
=======
# ICE-9 Visualization Project

**Author:** Sowjanya Teppali  
**Student ID:** 11857046  
**Course:** ICE-9 — Data Visualization  

**Tools Used:** Python (Jupyter Notebook), Altair, HTML, CSS  

---

## 1. Objective

The goal of this project is to study and visualize the company’s growth from **2018 to 2030** using several types of charts.  
The dataset includes **Revenue**, **Expenses**, **Profit**, and **Employees**, which collectively describe the organization’s overall performance.

---

## 2. Tools and Technologies

| Tool / Library | Purpose |
|----------------|----------|
| **Python (Jupyter Notebook)** | Data processing and analysis |
| **Altair** | Building interactive visualizations |
| **Pandas** | Handling and transforming data |
| **HTML / CSS** | Creating a multi-page interactive website |

---

## 3. Dataset

**Source:** `company_growth.csv`

| Column | Description |
|---------|-------------|
| Year | Year (2018–2030) |
| Revenue | Company revenue in millions |
| Expenses | Total expenses in millions |
| Profit | Profit in millions |
| Employees | Total number of employees |

---

## 4. Visualizations Created

### 1️⃣ Scatter Chart  
- Plots **Revenue vs Profit** with color representing **Year** and circle size showing **Employees**.  
- Built using Altair’s `mark_circle()` for easy interpretation and visual clarity.

### 2️⃣ Bar Charts  
- Displays **stacked** and **grouped** bars comparing **Revenue, Expenses, and Profit** each year.  
- Clearly demonstrates yearly performance variations.

### 3️⃣ Area and Line Charts  
- Area charts highlight **growth trends** of key metrics across years.  
- Line charts provide precise **year-to-year comparisons** for visual consistency.

---

## 5. Multi-Page Website Structure

| File | Description |
|------|--------------|
| `index.html` | Home page with introduction and navigation links |
| `scatter.html` | Contains scatter plot visualizations |
| `bar.html` | Displays both stacked and grouped bar charts |
| `line.html` | Includes area and line charts |
| `styles.css` | Manages consistent styling and animations |

All pages are connected through a common navigation bar for smooth access.

---

## 6. Styling Features

- Simple, clean layout with **gradient header** and **modern typography**  
- Smooth **fade-in animations** for charts and images  
- **Responsive design** that adapts to desktop and laptop screens  
- Soft **blue-white color palette** for a professional academic appearance

---

## 7. Observations and Insights

- Both **revenue** and **profit** show a steady upward trend between 2018 and 2030, reflecting continuous progress.  
- **Expenses** also rise over time but remain proportionate to revenue.  
- **Employee count** increases consistently, showing scalable and sustainable operations.

---

## 8. Folder Contents
```bash
    Kv_Store/
        ICE9-Visualization/
            │
            ├── data/
            │ └── company_growth.csv
            │
            ├── site/
            │ ├── index.html
            │ ├── scatter.html
            │ ├── bar.html
            │ ├── line.html
            │ └── styles.css
            │
            └── notebooks/
            └── ICE9_Visualization.ipynb

   ```

## 9. Summary of Results

| Visualization | Key Insight |
|----------------|-------------|
| **Scatter Chart** | Revenue strongly correlates with employee growth |
| **Bar Chart** | Clear comparison of yearly revenue, expenses, and profit |
| **Area Chart** | Demonstrates a continuous rise in overall financial performance |
| **Line Chart** | Displays smooth consistency in yearly growth trends |

---

## 10. Conclusion

The **ICE-9 Visualization Project** illustrates how data visualization can summarize financial information effectively.  
It combines **Python analytics** and a **multi-page website** built with **Altair and HTML/CSS**.  
The project demonstrates clear patterns of company expansion and highlights the value of visualization in business analysis.

---

**© 2025 Sowjanya Teppali — ICE-9 Project**

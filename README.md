# 💰 SplitEase – Smart Expense Splitter
*A simple yet thoughtful Google Sheets project that makes sharing expenses with my girlfriend effortless and fair.*

---

## 🌟 Overview
**SplitEase** is a cloud-based spreadsheet app I designed for personal use with my girlfriend 💑.  
It automatically calculates shared expenses, balances, and settlements — so we can focus on enjoying life, not math.  
Built entirely in **Google Sheets**, it combines spreadsheet logic, macros, and design polish into one clean interface.

---

## 🧩 Features
- 📊 **Organized Table Structure** – Track expenses by date, item, payer, ratio, and total.
- 🧠 **Smart Formulas** – Includes:
  - `IF` and nested `IF` for **three spending scenarios** (shared, individual, partial).
  - `SUMIF` for automatic total calculation by person.
  - Ratio-based formulas for flexible sharing logic.
- ⚙️ **Macro Automation** – A “Settle Up” button to summarize and reset values.
- 🎨 **User-Centered Design** – Color-coded highlights, clear totals, and visual feedback.
- 💵 **Instant Settlement Summary** – Displays who should pay whom and how much.

---

## 🧮 Formula Highlights
| Purpose | Formula | Description |
|----------|----------|-------------|
| Split amount calculation | `=Amount * Ratio` | Calculates each person’s share dynamically |
| Determine payer | `=IF(PaidBy="J", Amount*0.5, Amount*0)` | Allocates costs based on payer |
| Sum totals | `=SUMIF(PaidBy, "J", Total)` | Totals up by person automatically |
| Multi-scenario logic | `=IF(A="Shared", Amount/2, IF(A="T", Amount, 0))` | Handles 3 cases cleanly |

---

## 🖼 Preview
![Preview of SplitEase Sheet](assets/preview.png)
> Example showing expense list, ratios, and settlement summary (“T pays J $99.315”).

---

## 🚀 Live Demo
🔗 [**View Interactive Version**](https://yourusername.github.io/split-expense-tracker/)  
*(Hosted via GitHub Pages, embedded from Google Sheets.)*

---

## 🛠 Tech Stack
- **Google Sheets** – core logic and interface  
- **Apps Script Macro** – automation for the “Settle Up” button  
- **HTML + CSS** – embedding page design  
- **GitHub Pages** – hosting for public demo

---

## 💡 Project Story
This started as a way to make our daily expense tracking easier.  
I used it to practice spreadsheet logic and UI design — and it became something we use every week!  
It’s practical, clean, and built with love 💕  

Through this project, I learned how to:
- Use **formulas to handle different payment scenarios**
- Apply **conditional formatting** for clarity
- Design intuitive **macro-based interactions**

> 💬 *“A tiny sheet that keeps love (and math) balanced.”*

---

## 👤 Author
**Your Name**  
📧 [your.email@example.com]  
🐙 [GitHub Profile](https://github.com/yourusername)


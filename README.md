# Student Gradebook Manager 📚📊

An interactive, command-line interface (CLI) application developed in Python to manage student academic records, track performance, and calculate comprehensive classroom statistics. This project highlights efficient matrix operations and handling missing data dynamically using **NumPy**.

---

## 📌 Features
* **Grade Management Dashboard:** View all student names, raw scores, individual averages, and summary stats in a clean, structured table.
* **Dynamic Student Roster:** Add new students with individual grade hooks or remove existing ones seamlessly.
* **Scalable Assignments Architecture:** Expand the grade book dynamically by appending new quizzes or exams, updating the internal matrices for all current records.
* **Advanced Classroom Insights:** Instantly evaluate global benchmarks per assignment:
  * Class Averages (Handles missing values gracefully)
  * Peak and Minimum Scores (Max/Min)
  * Standard Deviation ($\sigma$) to measure data dispersion.

---

## 🛠️ Technical Highlights & Implementation
* **Robust Missing Data Handling:** Utilized specialized NumPy methods (`np.nanmean`, `np.nanstd`, `np.nanmax`, `np.nanmin`) to enable seamless execution even if a student missed an assignment (stored as `np.nan`), preventing system crashes or statistical skewing.
* **Array Manipulation:** Employed dynamic resizing methods like `np.append` and `np.delete` to manipulate internal matrices efficiently when assignments are added or dropped.
* **Defensive Programming & Input Validation:** Built strong `try-except` blocks and loop guards to sanitize user entries against negative scores, text in numeric fields, and duplicate records.

---

## 🧪 Computational Methods & Math Applied
The system performs calculations across rows and structural axes seamlessly:
1. **Student Performance:** Computed row-wise averages to track individual academic growth.
2. **Assignment Performance:** Utilized column-wise evaluation (`axis=0`) to calculate class statistics for each evaluation type individually.
3. **Standard Deviation:** Calculated using:
   $$\sigma = \sqrt{\frac{1}{N}\sum_{i=1}^{N}(x_i - \mu)^2}$$
   This helps instructors instantly spot the variance and complexity level of each exam or quiz.

---

## 📄 Project Context & Details
* **Institution:** University College of Applied Sciences (UCAS)
* **Course:** Programming Language for Data Science (Lab)
* **Section ID:** 201
* **Instructor:** Eng. Abd Elkarim Abu Samra
* **Developer:** Amal Ahmed Abu Elba
* **Student ID:** 220231850

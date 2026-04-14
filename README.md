# InsightShelf

<p align="center">
  <strong>Turning raw library transactions into student behavior insights.</strong>
</p>

<p align="center">
  A data mining notebook that cleans borrowing records, engineers meaningful features,
  visualizes reading behavior, and segments students into actionable engagement groups.
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Python-Data%20Mining-1f6feb?style=for-the-badge" alt="Python Data Mining badge" />
  <img src="https://img.shields.io/badge/Jupyter-Notebook-f59e0b?style=for-the-badge" alt="Jupyter Notebook badge" />
  <img src="https://img.shields.io/badge/ML-K--Means-0f766e?style=for-the-badge" alt="K-Means badge" />
  <img src="https://img.shields.io/badge/License-MIT-111827?style=for-the-badge" alt="MIT License badge" />
</p>

---

## What This Project Does

`InsightShelf` explores how students use a library system by transforming transactional borrowing data into interpretable patterns.

Inside the notebook, the workflow:

- normalizes inconsistent date fields
- calculates borrow duration
- builds per-student features such as `LibraryScore`
- identifies favorite reading categories
- standardizes data for machine learning
- segments students with K-Means clustering
- visualizes category, department, temporal, and engagement trends

This is not just a notebook full of charts. It is a compact behavioral analytics pipeline for understanding reader engagement.

---

## Why It Stands Out

Most academic data projects stop at summary statistics. This one pushes further by asking:

- Who are the power users of the library?
- Which students borrow frequently but return quickly?
- Which categories dominate borrowing habits?
- How do departments and reading preferences intersect?
- What patterns appear over time?

By combining feature engineering, clustering, and visual storytelling, the notebook turns a plain dataset into a narrative about student behavior.

---

## Core Analysis Pipeline

### 1. Data Cleaning

The notebook begins by parsing and normalizing `BorrowDate` and `ReturnDate`, ensuring reliable time-based analysis.

### 2. Feature Engineering

It derives several useful student-level signals:

- `LibraryScore`: number of books borrowed by each student
- `AverageBorrowDuration`: average number of days books are kept
- `FavoriteCategory`: most frequently borrowed category per student

### 3. Standardization

Numeric features are scaled so clustering is based on comparable dimensions rather than raw magnitude.

### 4. Student Segmentation

K-Means clustering groups students into three interpretable segments:

- `Occasional Borrowers`
- `Consistent Readers`
- `Power Users`

### 5. Visual Exploration

The notebook includes visual analysis for:

- distribution of library scores
- category popularity
- average borrow duration by category
- department vs. category heatmap
- cluster scatter visualization
- correlation between score and borrow duration
- monthly borrowing trends
- borrow duration spread across categories

---

## Project Structure

```text
.
|-- Data_Mining.ipynb
|-- LICENSE
`-- README.md
```

---

## Tech Stack

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- scikit-learn
- Jupyter Notebook / Google Colab

---

## How To Run

### Option 1: Jupyter Notebook

1. Clone this repository.
2. Open `Data_Mining.ipynb`.
3. Make sure your dataset is available and update the dataset path if needed.
4. Run the notebook cells in order.

### Option 2: Google Colab

1. Upload the notebook to Colab.
2. Upload your dataset file, typically as `dataset.csv`.
3. Update the path used in the notebook if your file location differs.
4. Execute all cells sequentially.

---

## Expected Dataset Fields

The notebook logic suggests the dataset should include columns similar to:

- `StudentID`
- `BorrowDate`
- `ReturnDate`
- `Category`
- `Department`

If your schema differs, adjust the notebook column references before running the analysis.

---

## Example Outcomes

With the provided workflow, you can uncover insights such as:

- which students are highly engaged with the library
- which content categories are most attractive
- whether certain departments prefer specific topics
- how long books are usually retained
- how borrowing activity changes across months

These results can support academic planning, collection strategy, and student engagement decisions.

---

## Who This Is For

This project is useful for:

- students building portfolio-ready data mining work
- educators demonstrating applied analytics
- librarians exploring usage intelligence
- beginners learning feature engineering and clustering

---

## Future Improvements

- add the source dataset to the repository
- export charts as report-ready images
- include model evaluation notes for cluster selection
- build an interactive dashboard version
- automate preprocessing with a standalone Python script

---

## License

This project is licensed under the MIT License. See [LICENSE](LICENSE).

---

## Final Note

If spreadsheets show what happened, `InsightShelf` shows what it means.

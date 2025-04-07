# Task-1-Elevate-labs
# 📊 Netflix Data Cleaning & Preprocessing

This repository contains a Python-based data cleaning and preprocessing workflow applied to a raw Netflix dataset. The dataset includes details about movies and TV shows available on Netflix, including title, type, cast, country, release year, rating, and more.

---

## 🧠 Objective

The goal of this project is to clean and prepare the raw dataset by:
- Handling missing values
- Removing duplicate entries
- Standardizing inconsistent text formats
- Converting columns to appropriate data types
- Renaming columns for consistency and readability

---

## 🛠️ Tools & Technologies

- **Python 3**
- **Pandas**
- Google colab Notebook 

---

## 📁 Dataset Description

The dataset `Netflix_movies_and_tv_shows_clustering.csv` includes the following columns:

| Column         | Description |
|----------------|-------------|
| show_id        | Unique identifier |
| type           | Movie or TV Show |
| title          | Title of the content |
| director       | Director name |
| cast           | Cast list |
| country        | Country of origin |
| date_added     | Date content was added |
| release_year   | Year of release |
| rating         | Age rating (e.g., PG, TV-MA) |
| duration       | Length of movie or show |
| listed_in      | Genre categories |
| description    | Summary of the content |

---

## 🧹 Cleaning Steps

### ✅ 1. **Handled Missing Values**
- Filled `director`, `cast`, `country`, `rating` with `"Unknown"`.
- Converted `date_added` to datetime format (`YYYY-MM-DD`), with invalid dates handled as `NaT`.

### ✅ 2. **Removed Duplicates**
- Used `.drop_duplicates()` to eliminate duplicate rows.

### ✅ 3. **Standardized Text Columns**
- Converted text fields (e.g., `type`, `country`, `rating`) to lowercase and removed extra spaces.

### ✅ 4. **Formatted Dates**
- Converted `date_added` column to a standard datetime format.

### ✅ 5. **Cleaned Column Names**
- Renamed all column headers to lowercase with underscores instead of spaces for better readability.

### ✅ 6. **Fixed Data Types**
- Ensured that `release_year` is of type `int`.

---

## 💾 Output

- Cleaned dataset saved as: [`cleaned_netflix_dataset.csv`](./cleaned_netflix_dataset.csv)

---


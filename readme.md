
# Trending YouTube Video Analysis (2025-26 Project)

This project analyzes the "Trending YouTube" dataset to uncover insights about viral videos across different countries. It is developed as a Jupyter Notebook for the 2025-26 course project.

## Project Structure

The project expects the following directory structure:

```text
├── data/
│   ├── csv/                
│   │   ├── CAvideos.csv
│   │   ├── USvideos.csv
│   │   └── ... 
│   └── json/               
│       ├── CA_category_id.json
│       ├── US_category_id.json
│       └── ...
├── code.ipynb               # Main Jupyter Notebook with analysis
├── README.md                # Project documentation

```

## Setup & Requirements

### Prerequisites

* Python 3.x
* Jupyter Notebook

### Installation

1. **Clone the repository** (if applicable):
```bash
git clone https://github.com/MuhammadAbbasi/FCS_Bicocca.git

```


2. **Install required libraries**:
```bash
pip install pandas numpy matplotlib seaborn

```


3. **Data Setup**:
* Download the dataset from [Google Drive](https://drive.google.com/file/d/1VuI1NnPzYlhHIMBy-2nBegFoQTATbf8K/view?usp=sharing).
* Unzip the contents.
* Move all `.csv` files into `data/csv/`.
* Move all `.json` files into `data/json/`.



## Project Objectives & Steps

This notebook executes the following 15 analysis steps:

1. **Data Consolidation**: Merging CSVs from `data/csv/` into a single dataframe with a `country` column.
2. **Missing Tags**: Identifying and counting videos with no tags.
3. **Channel Views**: Calculating total viewership per channel.
4. **Data Cleaning**: Removing rows with disabled comments/ratings or error flags.
5. **Engagement Ratio**: creating a `like_ratio` column (likes divided by dislikes).
6. **Time Clustering**: Grouping publish times into 10-minute intervals.
7. **Interval Stats**: Analyzing average likes/dislikes per time interval.
8. **Tag Frequency**: Counting the number of videos for every unique tag.
9. **Top Tags**: Identifying the tags with the highest video counts.
10. **Tag Sentiment**: Computing average like ratios for each (Tag, Country) pair.
11. **Trending Peaks**: Finding the most-viewed video for each trending date/country.
12. **Date Parsing**: Splitting `trending_date` into Year, Month, and Day.
13. **Monthly Highlights**: Identifying the top video per month for each country.
14. **Category Mapping**: Loading category names and assignability rules from `data/json/`.
15. **Unassignable Categories**: Counting videos with categories marked as "not assignable" or missing from the JSON definitions.

## AI Usage Declaration

* AI tools were used to assist in generating code snippets for data cleaning and visualization (specifically Matplotlib and Seaborn plots).

```

```
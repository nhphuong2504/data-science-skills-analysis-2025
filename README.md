# Data Science Job Market Skills Analysis

Analyze data science job postings to extract and analyze in-demand skills from job descriptions.

## Project Overview

This project analyzes job postings from Indeed to identify the most frequently mentioned skills in data science positions. It provides insights into:
- Most in-demand skills by category
- Skill trends over time
- Comparisons between similar tools/technologies
- Company distribution in the job market

## Project Structure

```
DS-job-market-skill-analysis/
├── data/
│   └── IndeedJobScraperIntern.csv    # Job postings dataset
├── notebooks/
│   └── exploration.ipynb             # Main analysis notebook
├── outputs/
│   └── top_20_skills_by_category.jpg # Visualization output
├── requirements.txt                   # Python dependencies
└── README.md                          # This file
```

## Installation

1. Clone or download this repository
2. Install required packages:
```bash
pip install -r requirements.txt
```

## Dependencies

- pandas
- numpy
- matplotlib

## Usage

1. Open the Jupyter notebook:
```bash
jupyter notebook notebooks/exploration.ipynb
```

2. Run the cells in order:
   - **Section 1**: Load and explore the dataset
   - **Section 2**: Define skills by category
   - **Section 3-4**: Calculate skill frequencies
   - **Section 5**: Generate visualizations
   - **Section 6-10**: Run specific analyses

## Analysis Features

### Skill Categories Analyzed

- **Programming**: Python, SQL, R, Java, JavaScript, etc.
- **Mathematics & Statistics**: Statistics, Probability, Optimization, etc.
- **Machine Learning**: Deep Learning, XGBoost, Random Forest, etc.
- **AI Agents & Generative AI**: LLMs, NLP, RAG, Prompt Engineering, etc.
- **Agentic Frameworks & Tools**: LangChain, CrewAI, AutoGen, etc.
- **Data Engineering & MLOps**: Docker, Kubernetes, Spark, Airflow, etc.
- **Database Systems**: PostgreSQL, MongoDB, Snowflake, BigQuery, etc.
- **Cloud**: AWS, Azure, Google Cloud
- **Visualization & BI**: Tableau, Power BI, Matplotlib, etc.
- **Professional Skills & Ethics**: Communication, Data Analysis, Problem-solving, etc.

### Key Analyses

1. **Skill Frequency Analysis**: Count how many jobs mention each skill
2. **Top 20 Skills Visualization**: Bar chart showing most frequent skills by category
3. **Monthly Trends**: Track skill popularity over time
4. **Skill Comparisons**: 
   - Python vs R
   - AWS vs Azure
   - Power BI vs Tableau
5. **Category Analysis**: Analyze jobs mentioning skills from specific categories
6. **Company Analysis**: Distribution of companies in the dataset

## Output Files

- `outputs/top_20_skills_by_category.jpg`: Visualization of top 20 most frequent skills

## Notes

- Each skill is counted only once per job posting, even if mentioned multiple times
- Skills with aliases (e.g., "Data Analysis" and "Data Analytics") are counted together
- Analysis uses case-insensitive matching with word boundaries to avoid false positives

## Data Source

The dataset contains job postings scraped from Indeed, focusing on data science and related positions.

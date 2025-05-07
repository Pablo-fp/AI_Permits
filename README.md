# Boston2025 Data Processing Pipeline, Original work by Yair Titelboim

This repository contains a Google Colab notebook that replicates the three-phase data processing pipeline for the Boston2025 project, which tests the hypothesis that traditional urban economic models underestimate cross-project network effects by 30-50% in Boston.

## Project Overview

The Boston2025 project analyzes the relationship between review activity and permit values in Boston census tracts. The project demonstrates how review activity can serve as a leading indicator of development activity, with a typical lag of 6 months.

## Pipeline Phases

1. **Phase 1: Data Collection and Processing**

   - Load census tract boundaries and pre-processed uplift data
   - Load and clean review data
   - Visualize baseline and uplift values by census tract

2. **Phase 2: LLM Analysis for Sentiment and Themes**

   - Load pre-processed LLM data with sentiment scores and themes
   - Analyze sentiment score distributions and top themes
   - Merge LLM results with tract boundaries
   - Visualize sentiment scores by census tract

3. **Phase 3: Uplift Analysis**
   - Load quarterly review counts and detect review pulse
   - Analyze uplift values and their relationship with review pulse
   - Identify correlations between review sentiment and permit uplift
   - Analyze the Seaport district as a key example of review activity preceding permit activity
   - Create summary dashboard visualizations

## Repository Structure

- `AI_Review_Permits_Pipeline.ipynb`: The main Colab notebook that implements the pipeline
- `data/`: Directory containing input data files
  - `boston-census-tracts.geojson`: Census tract boundaries for Boston
  - `tracts_reviews.json`: Raw review data by census tract
  - `tracts_reviews_llm.json`: LLM-processed sentiment scores and themes
  - `tracts_FY25_review_uplift.geojson`: Census tracts with baseline values, actual values, and uplift
  - `review_counts_by_tract.csv`: Quarterly review counts by tract
- `work/`: Directory for intermediate output files
- `visualizations/`: Directory for visualization outputs

## Key Findings

1. Traditional urban economic models underestimate cross-project network effects by 30-50% in Boston.
2. Review activity can serve as a leading indicator of development activity, with a typical lag of 6 months.
3. Tracts with review pulse show significantly higher uplift values compared to those without.
4. There is a positive correlation between review sentiment and permit value uplift.
5. The Seaport district provides a clear example of review activity preceding permit activity.

## How to Use

1. Upload the entire folder to Google Drive
2. Open the `AI_Review_Permits_Pipeline.ipynb` notebook in Google Colab
3. Run the notebook cells sequentially to reproduce the analysis
4. Visualizations will be saved to the `visualizations/` directory
5. Intermediate data files will be saved to the `work/` directory

## Requirements

- Python 3.6+
- pandas
- numpy
- geopandas
- matplotlib
- seaborn
- shapely
- openai (for LLM analysis)

## License

This project is for educational and research purposes only.

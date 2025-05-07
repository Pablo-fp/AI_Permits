# Phase 2 QA Report

## Data Processing Summary

- **Total census tracts**: 207
- **Tracts with LLM data**: 98
- **Tracts without LLM data**: 109

## Field Verification

| Field | Present | Values |
|-------|---------|--------|
| sentiment_score | ✓ | Range: 0.1 to 0.9 |
| top_themes | ✓ | List of themes |

## Sample Data

Here are 5 random tracts with their LLM-derived fields:

### Sample 1: GEOID 25025060501
- Sentiment Score: 0.30000000000000004
- Top Themes: Pharmacy service, Customer service, Clothing selection

### Sample 2: GEOID 25025092000
- Sentiment Score: 0.2
- Top Themes: pizza quality, delivery service, missing items

### Sample 3: GEOID 25025060301
- Sentiment Score: 0.6000000000000001
- Top Themes: groceries, service, bagels

### Sample 4: GEOID 25025020101
- Sentiment Score: 0.9
- Top Themes: park, customer service, shopping

### Sample 5: GEOID 25025020301
- Sentiment Score: 0.9
- Top Themes: nail tech, gel overlay, customer service

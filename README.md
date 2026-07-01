# Sales Territory Optimization using K-Means Clustering

## Project Overview

This project demonstrates how machine learning can be used to optimize sales territories by grouping customer locations into geographically compact regions while balancing sales potential. The project uses the SimpleMaps US ZIP Codes dataset and applies the K-Means clustering algorithm to generate optimal sales territories.

## Objectives

- Acquire a publicly available dataset containing customer location information.
- Preprocess geographical and sales-related data.
- Cluster customer locations into optimal sales territories.
- Assign sales representatives to each territory.
- Visualize territories on an interactive map.
- Export territory assignments to CSV and Excel files.

## Dataset

**Source:** SimpleMaps US ZIP Codes Database

https://simplemaps.com/data/us-zips

The dataset contains:
- ZIP Code
- City
- State
- Latitude
- Longitude
- Population

A hypothetical sales potential is generated using the population values.

## Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- Folium
- OpenPyXL

## Machine Learning Algorithm

The project uses **K-Means Clustering** to divide customer locations into multiple sales territories based on:

- Latitude
- Longitude
- Normalized Sales Potential

Each cluster represents one optimized sales territory.

## Workflow

1. Load the US ZIP Codes dataset.
2. Filter the dataset for California.
3. Clean missing values.
4. Generate a hypothetical sales potential.
5. Normalize sales potential using MinMaxScaler.
6. Apply K-Means clustering.
7. Assign a sales representative to each territory.
8. Visualize territories using Folium.
9. Export the final assignments to CSV and Excel.

## Output Files

After running the script, the following files are generated:

- `sales_territory_assignments.csv`
- `sales_territory_assignments.xlsx`
- `sales_territory_map.html`

## Installation

Install the required Python packages:

```bash
pip install pandas numpy scikit-learn folium openpyxl
```

## Running the Project

Place the dataset (`uszips.csv`) in the project directory or update the file path in the script.

Run:

```bash
python sales_territory_optimization.py
```

or execute the notebook cells if using Jupyter Notebook or Google Colab.

## Results

The project successfully:

- Creates optimized sales territories using K-Means clustering.
- Balances customer distribution across territories.
- Assigns one sales representative per territory.
- Produces an interactive geographic visualization.
- Exports the final territory assignments for business use.

## Project Structure

```
├── uszips.csv
├── sales_territory_optimization.py
├── sales_territory_assignments.csv
├── sales_territory_assignments.xlsx
├── sales_territory_map.html
└── README.md
```

## Future Improvements

- Incorporate actual customer revenue instead of simulated sales potential.
- Use weighted K-Means for improved workload balancing.
- Compare K-Means with DBSCAN and Hierarchical Clustering.
- Include travel distance optimization using road networks.
- Develop a web dashboard for interactive territory management.

## Author

Developed as part of a Sales Territory Optimization project using Python and Machine Learning.

## License

This project is intended for educational purposes.

Dataset Source:
SimpleMaps US ZIP Codes Database

https://simplemaps.com/data/us-zips

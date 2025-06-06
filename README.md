# Statistical Data Analysis with Python

A comprehensive statistical analysis project that explores three popular datasets using Python's data science libraries. This project demonstrates histogram analysis with normal distribution curves, correlation matrices, and box plots for exploratory data analysis.

## 📊 Datasets Analyzed

1. **Penguins Dataset** - Palmer Archipelago penguin data
2. **Iris Dataset** - Classic flower measurements dataset
3. **Planets Dataset** - Exoplanet discovery data

## 🛠️ Technologies Used

- **pandas** - Data analysis and manipulation
- **numpy** - Mathematical operations and array processing
- **plotly.graph_objects** - Interactive 3D visualizations
- **plotly.express** - High-level plotting interface
- **scipy.stats** - Statistical analysis tools (normal distribution, skewness)
- **seaborn** - Statistical data visualization (dataset loading)

## 📈 Analysis Features

### 1. Histogram Analysis with Normal Distribution
- Creates probability density histograms for all numeric columns
- Overlays normal distribution curves
- Calculates and displays skewness values
- Helps identify data distribution patterns

### 2. Correlation Matrix Heatmaps
- Generates correlation matrices for numeric features
- Interactive heatmaps with color coding
- Uses RdBu color scale for clear visualization
- Displays correlation coefficients as text overlays

### 3. Box Plot Analysis
- Creates box plots grouped by categorical variables
- Shows data distribution, outliers, and quartiles
- Includes all data points for detailed analysis
- Color-coded by categories for easy comparison

## 🚀 Getting Started

### Prerequisites

\`\`\`bash
pip install pandas numpy plotly scipy seaborn
\`\`\`

### Installation

1. Clone the repository:
\`\`\`bash
git clone <your-repository-url>
cd statistical-data-analysis
\`\`\`

2. Install required packages:
\`\`\`bash
pip install -r requirements.txt
\`\`\`

3. Run the analysis:
\`\`\`bash
python analysis.py
\`\`\`

## 📋 Code Structure

\`\`\`
├── analysis.py          # Main analysis script
├── README.md           # Project documentation
└── requirements.txt    # Python dependencies
\`\`\`

## 🔍 Analysis Workflow

1. **Data Loading & Preparation**
   - Load datasets using seaborn's built-in datasets
   - Remove missing values with `dropna()`
   - Identify numeric and categorical columns

2. **Statistical Analysis**
   - Generate histograms with normal distribution overlays
   - Calculate skewness for each numeric variable
   - Create correlation matrices for feature relationships

3. **Visualization**
   - Interactive plots using Plotly
   - Color-coded visualizations for better insights
   - Comprehensive box plots for categorical analysis

## 📊 Key Insights

### Penguins Dataset
- Analyzes bill length, bill depth, flipper length, and body mass
- Grouped by penguin species
- Reveals species-specific physical characteristics

### Iris Dataset
- Examines sepal and petal dimensions
- Classic dataset for classification analysis
- Shows clear species separation patterns

### Planets Dataset
- Studies orbital and physical properties of exoplanets
- Grouped by discovery method
- Reveals detection method biases and planet characteristics

## 🎯 Use Cases

- **Educational**: Learn statistical analysis techniques
- **Research**: Template for exploratory data analysis
- **Data Science**: Foundation for machine learning preprocessing
- **Visualization**: Examples of effective data presentation

## 📝 Features Explained

### Histogram Analysis
```python
# Creates probability density histograms
hist = g0.Histogram(x=data, histnorm='probability density')
# Overlays normal distribution curve
normal_curve = g0.Scatter(x=x_range, y=norm.pdf(x_range, mean, std))

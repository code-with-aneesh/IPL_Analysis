# IPL Data Analysis Project

## Project Overview
Python analysis of Indian Premier League (IPL) cricket data featuring:
- Team performance metrics
- Player statistics
- Match outcome analysis
- Venue-based trends

## Directory Structure
```text
ipl-analysis/
├── data/
│   ├── matches.csv
│   └── deliveries.csv
├── notebooks/
│   ├── match_analysis.ipynb
│   └── delivery_analysis.ipynb
└── README.md
```

## Installation
```bash
# Clone repository
git clone https://github.com/yourusername/ipl-analysis.git
cd ipl-analysis

# Create virtual environment
python -m venv venv
source venv/bin/activate  # Linux/Mac
.\venv\Scripts\activate   # Windows

# Install dependencies
pip install -r requirements.txt
```

## Example Analysis
```python
# Calculate top performing teams
import pandas as pd

matches = pd.read_csv('data/matches.csv')
top_teams = matches['winner'].value_counts().head(5)
print(top_teams)
```

## Contribution Guidelines
```bash
# Create new feature branch
git checkout -b feature/new-analysis
```

```python
# Function documentation example
def calculate_strike_rate(runs, balls):
    """
    Calculate batting strike rate
    
    Args:
        runs (int): Runs scored
        balls (int): Balls faced
        
    Returns:
        float: Strike rate (runs per 100 balls)
    """
    return (runs/balls)*100 if balls > 0 else 0
```

## License
MIT License

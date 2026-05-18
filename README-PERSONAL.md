# GA Dashboard - E-Commerce Trends and Insights

## 📊 Project Overview

This is a **personal fork** of the original [INFO-526-F24/project-01-Pacman](https://github.com/INFO-526-F24/project-01-Pacman) team project with **Google Analytics integration** added for enhanced website analytics tracking.

## 🆕 My Contributions

### Google Analytics Integration
- ✅ Added Google Analytics property setup and authentication
- ✅ Integrated Google Analytics Data API with R (`googleAnalyticsR` package)
- ✅ Created **"Website Analytics"** dashboard section with:
  - **Overall Web Metrics**: Active users, sessions, page views, engagement
  - **User Demographics**: Geographic distribution (countries), device types, operating systems
  - **Demo Data**: Displays sample data until real traffic arrives (24-48 hour delay)

### Technical Changes
- Added `googleAnalyticsR` package to dependencies
- Implemented service account authentication using `ga-credentials.json`
- Created automated data fetching and fallback to demo data
- Added responsive visualizations using ggplot2

## 📁 Original Project Details

**Original Repository**: [INFO-526-F24/project-01-Pacman](https://github.com/INFO-526-F24/project-01-Pacman)

**Original Team**: See contributors on the original repository

**Original Description**: Analysis of e-commerce trends and insights using retail store dataset with interactive visualizations.

## 🛠 Setup Instructions

### Requirements
- R 4.0+
- Quarto
- Google Analytics property and service account credentials

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/YOUR-USERNAME/ga-dashboard-pacman.git
   cd ga-dashboard-pacman
   ```

2. **Install R packages**
   ```r
   install.packages(c("googleAnalyticsR", "tidyverse", "scales", "ggplot2", 
                      "dlookr", "kableExtra", "gt", "gridExtra", "pacman"))
   ```

3. **Add Google Analytics credentials**
   - Obtain your `ga-credentials.json` from Google Cloud Console
   - Place it in the project root directory
   - Update the Measurement ID in `dashboard.qmd` (line with `GA_MEASUREMENT_ID`)

4. **Run the dashboard**
   ```bash
   quarto preview dashboard.qmd
   ```

## 📊 Dashboard Features

### Original Sections
- Overall metrics (orders, sales, profit, discounts)
- Sales by region visualization
- Profit by category analysis
- Top subcategories by sales

### New Analytics Sections
- **Website Analytics Dashboard** with:
  - Active users tracking
  - Session analytics
  - Page view metrics
  - Geographic user distribution
  - Device category breakdown
  - Operating system distribution

## ⚠️ Important Notes

- **Credentials**: `ga-credentials.json` is in `.gitignore` for security - keep it local
- **Data Delay**: Google Analytics data takes 24-48 hours to appear after first visit
- **Demo Data**: Dashboard displays sample data until real traffic arrives
- **Deployment**: Website must be publicly accessible for GA to collect data

## 📝 License

Same as the original project.

## 🤝 Credits

**Original Project Team**: [See original repository](https://github.com/INFO-526-F24/project-01-Pacman)

**GA Integration**: Personal enhancement by Devashree Pawar

---

**Note**: This is a personal fork created for educational purposes. For the original project, please visit the [INFO-526-F24/project-01-Pacman](https://github.com/INFO-526-F24/project-01-Pacman) repository.

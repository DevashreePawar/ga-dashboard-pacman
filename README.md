# Decoding E-Commerce Trends and Insights 📊

**Personal fork with Google Analytics Dashboard Integration**

## About This Project

This is an enhanced version of the INFO 526 Fall 2024 Project 1 with added **Google Analytics integration** for tracking website visitor demographics and engagement metrics.

### Original Project
- **Course**: INFO 526 - Data & Visualization
- **Institution**: University of Arizona
- **Team Project**: [Original Repository](https://github.com/INFO-526-F24/project-01-Pacman)
- **Original Focus**: E-Commerce trends analysis using retail store dataset

### ✨ New Features (Personal Addition)

**Google Analytics Dashboard Section:**
- 📍 **User Demographics**: Visitor countries, device types, operating systems
- 👥 **Engagement Metrics**: Active users, sessions, page views
- 📈 **Real-time Tracking**: Automatic data refresh from Google Analytics
- 🎨 **Interactive Visualizations**: Geographic distribution, device breakdown, OS trends

## 🚀 Quick Start

### Prerequisites
- R 4.0+
- Quarto
- Google Analytics credentials (see setup below)

### Installation

```bash
# Clone repo
git clone https://github.com/YOUR-USERNAME/ga-dashboard-pacman.git
cd ga-dashboard-pacman

# Install dependencies
R -e "install.packages(c('googleAnalyticsR', 'tidyverse', 'scales', 'ggplot2', 'dlookr', 'kableExtra', 'gt', 'gridExtra', 'pacman'))"
```

### Google Analytics Setup

1. **Create GA4 Property**: [analytics.google.com](https://analytics.google.com)
2. **Get Measurement ID**: `G-XXXXXXXXXX`
3. **Create Service Account**: [Google Cloud Console](https://console.cloud.google.com)
4. **Download JSON Credentials**: Save as `ga-credentials.json` in project root
5. **Update Dashboard**: Replace Measurement ID in `dashboard.qmd`

### Run Dashboard

```bash
quarto preview dashboard.qmd
```

## 📑 Project Structure

```
├── dashboard.qmd              # Main dashboard (E-Commerce + GA Analytics)
├── index.qmd                  # Home page
├── proposal.qmd               # Project proposal
├── presentation.qmd           # Presentation slides
├── about.qmd                  # About page
├── data/                      # Datasets
├── images/                    # Visualizations
├── ga-credentials.json        # GA authentication (NOT committed to git)
└── README.md                  # This file
```

## 📊 Dashboard Sections

### E-Commerce Analytics (Original)
- Total Orders, Sales, Profit, Discount metrics
- Sales by Region
- Profit by Category
- Top Subcategories

### Website Analytics (New - GA Integration)
- Active Users & Sessions tracking
- Page Views & Engagement
- Top Countries by Visitors
- Device Type Distribution
- Operating System Breakdown

## ⚠️ Important Security Notes

**DO NOT COMMIT `ga-credentials.json`**
- Credentials file is in `.gitignore`
- Keep your service account key private
- Never share your Google Cloud credentials

## 📚 Resources

- [Google Analytics 4 Documentation](https://support.google.com/analytics)
- [googleAnalyticsR Package](https://github.com/MarkEdmondson1234/googleAnalyticsR)
- [Quarto Documentation](https://quarto.org)

## 👥 Credits

**Original Team**: [See original repository](https://github.com/INFO-526-F24/project-01-Pacman)

**GA Integration & Dashboard Enhancement**: Devashree Pawar

#### Disclosure
Derived from the original course by Mine Çetinkaya-Rundel @ Duke University

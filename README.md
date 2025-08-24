# NBA Analytics Pipeline

A data analytics project that collects NBA game data, stores it in a SQL database, and visualizes insights in Power BI.  
The long-term goal is to evolve this into a predictive analytics system using machine learning.  

## 🚀 Features
- Ingest historical NBA game data from public sources (Kaggle, Basketball Reference, NBA APIs).  
- Store cleaned data in a SQL database (SQLite for MVP, PostgreSQL for scaling).  
- Build Power BI dashboards for:
  - Team and player performance
  - Win/loss trends
  - Efficiency statistics  
- Iterative roadmap towards predictive models for game outcomes and player performance.  

## 📂 Repository Structure
 (...)


## 🛠️ Tech Stack
- **Data**: Kaggle datasets, Basketball Reference, NBA APIs  
- **Database**: SQLite (MVP), PostgreSQL (future)  
- **ETL**: Python (`pandas`, `sqlalchemy`, `requests`)  
- **Visualization**: Power BI  
- **ML/AI (future)**: scikit-learn, XGBoost, PyTorch  

## 📊 Example Dashboards
- Player stats over time  
- Team win/loss by season  
- Efficiency and shooting metrics  

## 📌 Roadmap
1. MVP: Load Kaggle data → SQLite → Power BI dashboard  
2. Iteration 1: PostgreSQL + automated ETL pipeline  
3. Iteration 2: Daily updates via NBA API/web scraping  
4. Iteration 3: Advanced analytics (rolling averages, PER, trends)  
5. Iteration 4: Predictive ML models (game outcome, player stats)  
6. Iteration 5: Cloud deployment (AWS/GCP)


# NBA Analytics Project Plan

## 1. Project Overview
This project aims to create a robust NBA analytics system that evolves from descriptive analytics to predictive modeling. The initial MVP will focus on building a working pipeline that ingests historical game data, stores it in a SQL database, and presents insights through Power BI dashboards.  

In later iterations, real-time data ingestion and machine learning models will be integrated, allowing predictive analytics such as game outcome forecasts and player performance predictions.  

---

## 2. Objectives
- **MVP Goal**: Build an end-to-end pipeline from data ingestion → SQL database → Power BI dashboard.  
- **Long-Term Goal**: Create a production-ready analytics system with machine learning predictors and automated cloud deployment.  

---

## 3. Methodology & Phases

### Phase 1: MVP – Historical Data to SQLite
- Data Source: Kaggle NBA datasets / Basketball Reference CSV exports.  
- ETL:
  - Python script to clean and load CSV into SQLite.  
  - Basic schema: `games`, `players`, `teams`, `box_scores`.  
- Dashboard:  
  - Power BI connected to SQLite.  
  - Visuals: win/loss %, average points per game, simple player stats.  

### Phase 2: Iteration – Database Upgrade & Automation
- Migrate database from SQLite → PostgreSQL.  
- Write automated ETL (Python + cron/Task Scheduler).  
- Expand schema with `play_by_play` table.  
- Power BI dashboards with more advanced KPIs (efficiency, shooting %).  

### Phase 3: Iteration – Real-Time Data Ingestion
- Replace static Kaggle datasets with NBA API / web scraping.  
- Daily ingestion pipeline that automatically updates database.  
- Power BI refresh scheduled daily.  

### Phase 4: Iteration – Advanced Analytics
- Add derived stats:
  - Player Efficiency Rating (PER).  
  - Rolling averages (last 5 games).  
  - Home vs Away splits.  
- Power BI interactive filters (season, player, team).  

### Phase 5: Iteration – ML/AI Predictor
- Export historical game-level data from PostgreSQL → Pandas.  
- Train initial ML models:
  - Logistic Regression / Random Forest for win/loss.  
  - Regression models for player scoring/rebounding forecasts.  
- Validate with accuracy/precision metrics.  
- Integrate results back into Power BI dashboards.  

### Phase 6: Production Deployment
- Cloud-hosted database (AWS RDS or GCP Cloud SQL).  
- ETL orchestrated with Airflow / Prefect.  
- Power BI dashboards shared online.  
- (Optional) Expose ML models via REST API (Flask/FastAPI).  

---

## 4. System Architecture (Conceptual)



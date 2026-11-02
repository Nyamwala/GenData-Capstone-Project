# East African Automotive Import Analytics & Logistics Dashboard

A comprehensive data analytics project designed for the Kenyan and East African automotive import industry. This project analyzes structured vehicle catalog data and export logs (**8,832+ records**) to optimize vehicle sourcing, track trade metrics, and model landed costs through Tableau.

## 🚀 The Problem We Are Solving

Importing used vehicles into East Africa (routed primarily through Mombasa Port) is often a financial guessing game. Dealerships and individual buyers face unpredictable cost structures where FOB vehicle prices, volatile ocean freight rates, mandatory pre-export inspection fees, and marine insurance fluctuate independently. Without a centralized data model, stakeholders frequently suffer compressed profit margins and unexpected capital shortfalls because they cannot accurately forecast total landed costs (CIF) before committing funds.

## 🛠️ Tools Used & What They Did

* **Python & Pandas**: Used for cleaning, structuring, transforming, and merging raw automotive inventory with historical shipping and logistics logs into unified, high-performance CSV datasets.
* **Tableau**: Developed interactive visual dashboards to analyze pricing tiers, mileage trade-offs, regional transit corridors, and destination markets across Kenya, Uganda, Tanzania, and DRC.
* **VS Code & Git Bash**: Served as the core development environment for writing data processing scripts, handling file paths, and managing project version control.

## 💡 Insights Discovered & Solutions Offered

### **The Insight**
Analyzing our curated dataset uncovered a hidden financial penalty in budget imports: because ocean freight and inspection fees are largely flat-rate charges, they inflate the landed cost of entry-level economy cars (like the Toyota Passo or Mazda Demio) disproportionately higher than high-end SUVs, heavily skewing true affordability for budget-conscious buyers.

### **The Solution**
* **Centralized Data Architecture:** Combined master vehicle records and relational export/pricing logs into a clean, query-ready format.
* **Accurate Landed Cost Modeling:** Integrated FOB vehicle prices with real-world shipping, port, and inspection logistics.
* **Interactive BI Dashboards:** Empowered car importers and dealerships to simulate total expenses before purchasing, protecting profit margins and eliminating guesswork.

## 📂 Project Structure

```
SBT-Japan-Analytics/
│
├── data/
│   ├── sbtjapan.csv                 # Master vehicle catalog dataset
│   └── sbt_pricing_and_export_logs.csv  # Relational export and logistics logs (8,832 rows)
├── notebooks/                       # Data processing and exploration notebooks
├── assets/                          # Tableau dashboard screenshots and visuals
└── README.md                        # Project documentation
```

## 📊 Getting Started & Tableau Integration

1. **Clone the repository:**
   ```bash
   git clone https://github.com/your-username/east-africa-auto-analytics.git
   cd east-africa-auto-analytics
   ```

2. **Prepare Your Data:**
   Ensure your master vehicle file and `sbt_pricing_and_export_logs.csv` are placed inside the `data/` directory.

3. **Connect in Tableau:**
   * Open Tableau Desktop.
   * Connect to text file and load `sbtjapan.csv` and `sbt_pricing_and_export_logs.csv`.
   * Establish a relational join between the two tables using **`stock_id`** and **car names** as the common keys.
   * Build your cross-border pricing and market demand dashboards!
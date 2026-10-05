# Sectoral Balances and Flow of Funds (2007–2025)
🚀 **[Visualizza la Dashboard Live](https://cmf666cmf.github.io/sectorial-balances-and-flow-of-funds/)**

An interactive **D3.js** dashboard designed to analyze macroeconomic trends and sectoral balance dynamics across six major global economies (Italy, USA, Luxembourg, Norway, Ireland, China) over the 2007–2025 timeframe.

---

## 📌 Theoretical Framework
The project is built upon the fundamental accounting identity of sectoral balances:

$$(S - I) \equiv (T - G - TR) + CA$$

Where:
- **(S − I)**: Private sector net balance (Savings − Investment)
- **(T − G − TR)**: Primary public sector balance (Taxes − Government Spending − Transfers)
- **CA**: Current Account balance

---

## 📊 Reading the Diagram
- **X-Axis**: Current Account balance (CA) as a % of GDP.
- **Y-Axis**: Primary public sector balance as a % of GDP.
- **Bisector ($S = I$)**: Represents the private sector break-even line. The vertical distance from a point to the bisector measures the private sector balance:
  - **Below the bisector**: Private sector surplus ($S > I$).
  - **Above the bisector**: Private sector deficit ($S < I$).

---

## ⚙️ Key Features
- **Dynamic Scatter Plot (D3.js)**: Continuous tracking of historical country trajectories by interpolating data across 5 anchor points (2007, 2010, 2015, 2020, 2025).
- **Animation & Timeline Controls**: Automatic playback ("Play/Pause"), step-by-step navigation, and interactive timeline slider (2007–2025).
- **Multiple Country Isolation**: Select individual countries or isolate multiple countries (`Ctrl/Cmd + Click`) to highlight specific trajectories for targeted comparison.
- **Real-Time Stats & Sparklines**: Real-time average calculations for sectors and dynamic sparkline charts in the sidebar.
- **2007 vs 2025 Comparison**: Summary view showing percentage point variations in private balances for each country.
- **Interactive Data Table**: Automatic column highlighting corresponding to the selected year.
- **Graphic Export**: Download the current diagram view as a vector `.svg` file.
- **Keyboard Shortcuts**:
  - `Space`: Play / Pause animation
  - `←` / `→`: Navigate to previous / next year
  - `R`: Reset animation to the initial year
  - `Esc`: Reset isolation filters

---

## 🛠️ Tech Stack & Data Sources
- **Frontend**: HTML5, CSS3 (Custom Properties, Dark Theme), JavaScript ES6+
- **Data Visualization**: [D3.js (v7)](https://d3js.org/)
- **Data Sources**: Eurostat, OECD, IMF WEO

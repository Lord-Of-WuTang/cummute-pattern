# 🚌 Lagos Commute Pulse: Visualized 🌆

A comprehensive data analysis tool that generates realistic Lagos commute data and creates engaging visualizations to understand transportation patterns, weather impacts, and commuter experiences across Nigeria's commercial hub.

## 🌟 Features

- **Realistic Data Generation**: Creates authentic Lagos commute scenarios with 7 start locations, 7 destinations, and 6 transport modes
- **Weather Impact Analysis**: Simulates how Lagos' weather affects commute times
- **Mood Tracking**: Correlates commute duration with commuter satisfaction levels
- **Interactive Dashboard**: 6 comprehensive visualizations in a single dashboard view
- **Statistical Insights**: Automated generation of key metrics and trends

## 🎯 What This Tool Analyzes

### Transport Modes
- **Bus** 🚌 - Most popular public transport
- **Okada** 🏍️ - Motorcycle taxis
- **Keke** 🛺 - Tricycle taxis (Keke NAPEP)
- **Car** 🚗 - Private vehicles
- **Ferry** ⛵ - Water transport
- **Walking** 🚶 - On foot

### Key Locations
**Start Points**: Ikeja, Yaba, Lekki, Surulere, Ajah, Victoria Island, Ikorodu
**Destinations**: CMS, Obalende, Oshodi, Apapa, Festac, Mile 2, Ojota

### Data Points Tracked
- Journey duration (minutes)
- Weather conditions (Sunny ☀️, Rainy 🌧️, Cloudy ☁️)
- Day of week (Monday-Friday)
- Commuter mood (Happy 🙂, Neutral 😐, Frustrated 😩)

## 📊 Visualizations Generated

1. **🕐 Travel Time by Weather**: Violin plots showing duration distribution across weather conditions
2. **😊 Weekly Mood Tracker**: Stacked bar chart of commuter satisfaction by day
3. **🗺️ Route Duration Heatmap**: Average travel times between all location pairs
4. **🚌 Transport Mode Distribution**: Donut chart showing mode popularity
5. **📅 Daily Average Commute Times**: Bar chart with error bars for weekly patterns
6. **⛅ Weather Impact Analysis**: Grouped bars showing how weather affects each transport mode

## 🚀 Quick Start

### Prerequisites
```bash
pip install pandas matplotlib seaborn numpy
```

### Usage
1. **Generate Data & Visualizations**:
   ```python
   python lagos_commute_enhanced.py
   ```

2. **Output**:
   - `lagos_commute_pulse.csv` - Generated dataset
   - Comprehensive dashboard with 6 visualizations
   - Statistical summary in terminal

### Sample Output Statistics
```
📊 LAGOS COMMUTE PULSE - SUMMARY STATISTICS
==================================================
📈 Total Commutes Analyzed: 200
⏱️ Average Commute Time: 52.3 minutes
😩 Longest Commute: 125 minutes
😊 Shortest Commute: 20 minutes
🌧️ Rain Delay Impact: +18.2 minutes
🚌 Most Popular Transport: Bus
📅 Worst Commute Day: Friday
🎯 Commuter Satisfaction: 34.5% happy commuters
```

## 🔍 Data Generation Logic

### Realistic Timing
- **Base Duration**: 20-90 minutes (realistic Lagos ranges)
- **Weather Penalty**: +10-30 minutes for rainy conditions
- **Mode Adjustments**: Walking and ferry get +5-15 minutes

### Mood Correlation
- 🙂 **Happy**: < 40 minutes
- 😐 **Neutral**: 40-69 minutes  
- 😩 **Frustrated**: 70+ minutes

## 📈 Use Cases

- **Urban Planning**: Understand traffic patterns and bottlenecks
- **Transportation Policy**: Analyze mode effectiveness and weather resilience
- **Business Intelligence**: Optimize delivery routes and timing
- **Academic Research**: Study commuter behavior and satisfaction
- **Data Science Education**: Practice with realistic, structured datasets

## 🛠️ Customization Options

### Modify Data Generation
```python
# Change sample size
df = generate_commute_data(n=500)

# Add new locations
start_locations = ['Ikeja', 'Yaba', 'Your_Location']

# Adjust weather impact
if weather == 'rainy':
    base_time += random.randint(15, 45)  # Increase penalty
```

### Visualization Tweaks
```python
# Change color schemes
colors = ['#Your_Color_Hex', '#Another_Color']

# Modify figure size
fig = plt.figure(figsize=(24, 18))  # Larger dashboard
```

## 📁 File Structure
```
├── lagos_commute_enhanced.py    
├── lagos_commute_pulse.csv 
├── Figure_R.png    
└── README.md                   
```

## 🎨 Design Philosophy

This tool prioritizes:
- **Visual Engagement**: Rich colors, emojis, and varied chart types
- **Real-world Relevance**: Based on actual Lagos transport scenarios
- **Statistical Rigor**: Proper error bars, correlation analysis
- **Actionable Insights**: Clear takeaways for decision-making

## 🤝 Contributing

Want to enhance this tool? Consider adding:
- **Time of day analysis** (peak hours vs off-peak)
- **Cost analysis** by transport mode
- **Environmental impact** calculations
- **Route optimization** algorithms
- **Seasonal variations** beyond daily weather

## 📝 License

Open source - feel free to adapt for other cities or use cases!

## 🏙️ About Lagos Context

Lagos, Nigeria's economic capital with 15+ million residents, faces unique transportation challenges. This tool captures the reality of daily commutes across:
- **Island-Mainland connectivity** via bridges
- **Mixed transport ecosystem** from modern to traditional
- **Weather sensitivity** during rainy seasons
- **High population density** creating traffic congestion

Perfect for understanding urban mobility in rapidly growing African cities!

---

*Built with ❤️ by MOKA! for Lagos commuters and urban data enthusiasts*



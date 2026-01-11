# SD Visualization - Build Spec

**Purpose:** Interactive web app demonstrating standard deviation using real stock data.

---

## Overview

Build a Flask application that:
1. Fetches historical stock data for two user-specified symbols
2. Displays an interactive, step-through visualization of how SD is calculated
3. Allows comparison between two stocks (absolute SD and percentage volatility)

---

## User Interface

### Input Controls
- [ ] Text input for Stock 1 symbol (default: SO)
- [ ] Text input for Stock 2 symbol (default: AAPL)
- [ ] Number input for weeks of data (default: 20)
- [ ] "Fetch Data" button to retrieve stock prices
- [ ] "Next Step" button to advance visualization

### Chart Area
- [ ] X-axis: Time (weeks)
- [ ] Y-axis: Price ($)
- [ ] Stock 1 displayed as green dots
- [ ] Stock 2 displayed as blue dots

### Computation Display
- [ ] Table showing: data point, deviation from mean, squared deviation
- [ ] Running calculation display
- [ ] Final SD result prominently shown

---

## Visualization Sequence

### Phase 1: Stock 1 (slower, educational pace)
1. [ ] Plot Stock 1 closing prices as green dots
2. [ ] Draw horizontal line at mean (labeled with value)
3. [ ] Animate vertical lines from each dot to mean line
4. [ ] Show computation table with deviations
5. [ ] Display final SD value for Stock 1

### Phase 2: Stock 2 (faster pace)
6. [ ] Plot Stock 2 closing prices as blue dots
7. [ ] Draw mean line for Stock 2
8. [ ] Show deviation lines (quicker animation)
9. [ ] Show computation table
10. [ ] Display final SD value for Stock 2

### Phase 3: Comparison
11. [ ] Show side-by-side summary:
    - Absolute SD for each stock
    - Coefficient of variation (SD/mean as %) for each stock
    - Which has more volatility in absolute terms?
    - Which has more volatility in relative terms?

---

## Technical Requirements

### Backend (Python/Flask)
- [ ] Flask app with routes for:
  - `/` - main page
  - `/api/fetch-stock` - fetch stock data given symbol and weeks
- [ ] Stock data fetching (use yfinance or Alpha Vantage)
- [ ] Calculate mean and SD server-side
- [ ] Return JSON with: prices, dates, mean, deviations, SD

### Frontend (HTML/JS)
- [ ] Single page application
- [ ] Chart library (Plotly.js or Chart.js)
- [ ] Step-through state machine for visualization phases
- [ ] Clean, minimal styling (no framework required, or use simple CSS)

### Data Format
```json
{
  "symbol": "SO",
  "prices": [72.50, 73.10, ...],
  "dates": ["2025-08-01", "2025-08-08", ...],
  "mean": 74.25,
  "deviations": [-1.75, -1.15, ...],
  "squared_deviations": [3.06, 1.32, ...],
  "sd": 2.84,
  "cv_percent": 3.82
}
```

---

## File Structure

```
sd-visualization/
├── app.py              # Flask application
├── static/
│   ├── style.css       # Minimal styling
│   └── app.js          # Frontend logic & chart
├── templates/
│   └── index.html      # Main page
├── requirements.txt    # Python dependencies
└── README.md           # Setup instructions
```

---

## Dependencies

```
flask
yfinance
```

---

## Visual Style

- Clean white background
- Minimal UI chrome
- Green (#22c55e) for Stock 1
- Blue (#3b82f6) for Stock 2
- Clear typography for numbers
- Mean line: dashed, same color as dots
- Deviation lines: lighter shade, thin

---

## Success Criteria

1. User can enter any two stock symbols
2. Visualization clearly shows SD is about distance from mean (horizontal), not trend
3. Step-through pacing allows understanding each phase
4. Comparison reveals relationship between price level and volatility
5. App runs locally with `python app.py`

---

## Notes for Claude Code

When building this:
- Start with a working Flask skeleton before adding complexity
- Get data fetching working first, then build visualization
- Test with SO and AAPL as default symbols
- Keep the step-through logic simple (array of phases, index pointer)
- Prioritize clarity over polish in first iteration

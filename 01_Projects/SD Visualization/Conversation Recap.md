# SD Visualization - Conversation Recap

**Date:** 2026-01-10
**Status:** Planning complete, ready to build

---

## Origin

This project emerged from a conversation where a friend (an economist) drew a diagram to explain standard deviation. The diagram showed a slanted regression-style line through data points—but that's not what SD is. SD measures spread around the **mean** (a horizontal line), not deviation from a trend.

Goal: Create a visualization that correctly demonstrates what standard deviation actually is.

---

## Core Insight to Communicate

**Standard deviation measures how spread out data points are from their average (mean).**

- The mean is a single number—a horizontal line on a chart
- SD is about distance from that flat line, not from a sloped trend
- A regression line answers "what's the trend?"
- SD answers "how scattered are the points around their center?"

---

## The Formula

$$s = \sqrt{\frac{1}{n-1} \sum_{i=1}^{n} (x_i - \bar{x})^2}$$

In plain English:
1. Calculate the mean (average)
2. For each point, measure distance from mean
3. Square those distances
4. Average the squared distances
5. Take the square root

---

## Design Decisions

### Data
- **Two stocks:** SO (Southern Company, lower price ~$70-90) and AAPL (Apple, higher price ~$200+)
- **Dynamic input:** User enters stock symbols in a text box
- **Parameterized:** User chooses how many weeks of data (default: 20)
- **Source:** Fetched via API at runtime

### Visualization Sequence

**Stock 1 (SO - green dots):**
1. Plot weekly closing prices as dots
2. Draw horizontal line at the mean
3. Show vertical lines from each dot to the mean (the deviations)
4. Display computation table: each deviation, squared deviation
5. Show final SD result

**Stock 2 (AAPL - blue dots):**
- Same sequence, but paced faster
- Allows comparison of absolute SD vs percentage volatility

### Technical Approach
- **Backend:** Python with Flask
- **Frontend:** Interactive HTML page with step-through reveal
- **Chart library:** Claude's choice (likely Plotly or Chart.js)
- **Visual style:** Clean and minimal

---

## Hypotheses to Test

1. Does the higher-priced stock (AAPL) have a larger absolute SD?
2. Do the two stocks have similar or different volatility in percentage terms (coefficient of variation = SD/mean)?

---

## Next Steps

See [[Build Spec]] for implementation requirements.

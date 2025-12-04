# Weekly Bitcoin Analysis Workflow

## Overview

> **🚀 NEW: Automated Workflow Available!**  
> For a faster, automated approach where the AI does most of the work, use `run_weekly_analysis.md` instead.  
> This manual workflow is for users who prefer full control over each step.

This document outlines the complete step-by-step manual process for conducting and documenting your weekly Bitcoin market peak predictions.

**Recommended Day:** Every Wednesday (to maintain consistency)  
**Estimated Time:** 45-60 minutes (manual) or 10-15 minutes (automated)  
**Required:** Internet access, AI assistant access (Claude, ChatGPT, etc.)

---

## Pre-Analysis Preparation (15 minutes)

### Step 1: Gather Current Market Data

#### Essential Metrics to Collect:
1. **Current BTC Price**
   - Source: [CoinMarketCap](https://coinmarketcap.com) or [CoinGecko](https://www.coingecko.com)
   - Note: 24h high/low, 7-day change

2. **Days Post-Halving**
   - Last halving: April 20, 2024
   - Calculate: Days from halving to current date
   - Formula: `(Current Date - April 20, 2024) in days`

3. **On-Chain Metrics**
   - **MVRV Ratio**: [Glassnode](https://glassnode.com) or [CryptoQuant](https://cryptoquant.com)
   - **NUPL**: [Glassnode](https://glassnode.com)
   - **Exchange Whale Ratio**: [CryptoQuant](https://cryptoquant.com)
   - **Exchange Flows**: Net inflows/outflows

4. **ETF Data**
   - **Weekly flows**: [SoSoValue](https://sosovalue.xyz)
   - **Cumulative inflows**: Year-to-date total
   - **Daily flow trends**: Last 5-7 days

5. **Macroeconomic Data**
   - **Fed Funds Rate**: [Federal Reserve](https://www.federalreserve.gov)
   - **Next FOMC decision probability**: [CME FedWatch](https://www.cmegroup.com/markets/interest-rates/cme-fedwatch-tool.html)
   - **Latest CPI/PCE**: [BLS](https://www.bls.gov/cpi/)
   - **DXY (USD Index)**: [TradingView](https://www.tradingview.com)

6. **Sentiment Indicators**
   - **Fear & Greed Index**: [Alternative.me](https://alternative.me/crypto/fear-and-greed-index/)
   - **Google Trends**: Bitcoin search volume
   - **Social sentiment**: [LunarCrush](https://lunarcrush.com) (optional)

### Step 2: Review Last Week's Analysis

1. Open `analysis_tracking.md`
2. Review previous week's prediction:
   - What was predicted peak date?
   - What was predicted peak price?
   - What was confidence level?
3. Check if any intermediate milestones were hit or missed
4. Note any significant events that occurred

### Step 3: Document Weekly Events

Create a list of significant events from the past 7 days:
- Major price movements (>10% swings)
- Regulatory announcements
- ETF flow changes (large outflows/inflows)
- Fed announcements or speeches
- Geopolitical events affecting markets
- Major institutional announcements
- Protocol upgrades or issues

---

## Analysis Execution (20-30 minutes)

### Step 4: Update Variables in Tracking Document

Open `analysis_tracking.md` and update the "Current Variables" section:

```markdown
### Week of [Current Date]

#### Market Variables
- **{{CURRENT_DATE}}**: [Today's date]
- **{{CURRENT_PRICE}}**: $[Current BTC price]
- **{{DAYS_POST_HALVING}}**: [Calculated days]
- **{{PREVIOUS_PEAK_DATE}}**: [Last week's prediction date]
- **{{PREVIOUS_PEAK_PRICE}}**: [Last week's prediction price]

#### Portfolio Variables
- **{{CURRENT_BTC_PERCENTAGE}}**: [Current BTC %]
- **{{CURRENT_USDT_PERCENTAGE}}**: [Current USDT %]
- **{{PORTFOLIO_VALUE}}**: [Optional total value]
- **{{LAST_ACTION}}**: [Last week's recommendation]
- **{{LAST_REBALANCE_DATE}}**: [Date of last rebalance]
```

### Step 5: Prepare the Prompt

Open `prompt.md` and do one of the following:

**Option A: Direct Substitution**
- Replace all `{{VARIABLES}}` with actual values
- Copy the entire updated prompt

**Option B: Context Addition**
- Keep variables as placeholders
- Add a context block at the top with current values:
  ```
  CURRENT CONTEXT:
  - Date: December 11, 2025
  - BTC Price: $95,000
  - Days Post-Halving: 601
  - Previous Prediction: Sept 15, 2026 at $165K
  ```

### Step 6: Run the Analysis

1. **Choose your AI platform**: Claude, ChatGPT, Gemini, etc.
2. **Paste the prompt** (with variables filled or context added)
3. **Attach relevant data** if your AI supports file uploads:
   - Previous week's analysis file
   - Any charts or graphs you've collected
4. **Submit and wait** for the comprehensive analysis

### Step 7: Review AI Output

Check that the analysis includes:
- ✅ Executive summary with clear prediction
- ✅ All required analysis sections
- ✅ Base/Bull/Bear case scenarios
- ✅ Probability distributions
- ✅ Catalyst and risk factors
- ✅ Key levels to monitor
- ✅ Weekly tracking metrics
- ✅ Portfolio Allocation Recommendation (action, targets, rationale, DCA integration, risk parameters)
- ✅ Week-over-week comparison (if not first analysis)

If anything is missing, ask follow-up questions to complete the analysis.

---

## Post-Analysis Documentation (10-15 minutes)

### Step 8: Save the Analysis

1. **Create filename**: `analysisMMDDYYYY.md`
   - Format: Month (2 digits), Day (2 digits), Year (4 digits)
   - Example: `analysis12042025.md` for December 4, 2025

2. **Save the file** in your working directory

3. **Quick review**: Ensure markdown formatting is correct

### Step 9: Update Analysis Tracking Log

Open `analysis_tracking.md` and update:

#### A. Prediction History Log Table
Add new row:
```markdown
| Dec 11, 2025 | Sept 20, 2026 (±3w) | $170K ($155-185K) | 58% | Active | Adjusted up due to positive ETF flows |
```

#### A2. Allocation Recommendation Log (new)
Record the weekly action and targets:
```markdown
| Week Of    | Action     | Target BTC % | Target USDT % | Rationale (1-2 lines)                 |
|------------|------------|--------------|---------------|---------------------------------------|
| Dec 11, 25 | BUY +10%   | 70%          | 30%           | Mid-cycle, supportive flows, MVRV 1.8 |
```

#### B. Key Events Timeline
Add any new significant upcoming events

#### C. Weekly Milestones & Accuracy Checks
Update checkboxes for completed milestones:
```markdown
- [x] FOMC decision (Dec 9-10) - Result: 25bps cut approved
- [ ] BTC reclaims $97,100 (bullish confirmation)
```

#### D. Week-Over-Week Changes Log
Fill in the comparison section:
```markdown
### Week of December 11, 2025

**Changes from last week:**
- Prediction date: Shifted 5 days later (Sept 15 → Sept 20)
- Prediction price: Increased $5K ($165K → $170K)
- Confidence level: Increased 3% (55% → 58%)

**New data that influenced changes:**
- ETF inflows turned positive: $1.2B inflow this week
- Fed confirmed 25bps cut as expected
- MVRV ratio increased from 1.8 to 2.1

**Key events this week:**
- FOMC cut rates by 25bps (Dec 10)
- BlackRock added $500M to IBIT
- BTC broke above $95K resistance
```

### Step 10: Update Milestones in Tracking

Review and update the status of:
- Short-term milestones (next 4 weeks)
- Medium-term milestones (Q1 2026)
- Long-term milestones (Q2-Q3 2026)

Check invalidation triggers:
- Has any bear case trigger been activated?
- Do we need to adjust the base case?

---

## Quality Control & Reflection (5-10 minutes)

### Step 11: Sanity Check

Ask yourself:
- ✅ Does the prediction make logical sense given current data?
- ✅ Is the prediction internally consistent?
- ✅ Are probabilities properly distributed (should sum to ~100%)?
- ✅ Have I documented all significant changes?
- ✅ Are data sources cited and verifiable?

### Step 12: Document Insights

In `analysis_tracking.md`, update the "Notes & Insights" section:

```markdown
## Notes & Insights

### What's Working
- ETF flow tracking has been highly predictive
- Fed policy indicators correlating well with price action

### What Needs Improvement
- Need better sentiment indicators
- Social media sentiment less reliable than expected

### Black Swan Considerations
- Watch for potential Q1 2026 government shutdown
- Strategic Bitcoin Reserve legislation gaining momentum
```

### Step 13: Execute Portfolio Recommendation (Optional)

If you plan to follow the allocation recommendation:

**Review the Recommendation:**
- Action type (BUY/SELL/HOLD/DCA ONLY)
- Target allocation percentages
- Rationale and risk parameters
- DCA integration notes

**Before Executing:**
- ✅ Confirm recommendation aligns with your risk tolerance
- ✅ Check current exchange prices (may differ from analysis price)
- ✅ Verify sufficient liquidity and reasonable fees
- ✅ Review stop-loss and take-profit triggers
- ✅ Document your decision (follow, modify, or skip)

**Execution Options:**

1. **Immediate Execution** (same day as analysis)
   - Best for significant market changes
   - Execute full adjustment at current price

2. **Time-Weighted Execution** (over 2-7 days)
   - Split the allocation change over multiple days
   - Reduces timing risk
   - Example: +10% BTC = +2% per day for 5 days

3. **Limit Order Execution** (wait for better price)
   - Set limit orders at target prices
   - May not fill if market moves against you

4. **DCA Only** (ignore tactical overlay)
   - Stick to base DCA regardless of recommendation
   - Most conservative approach

**Record Execution:**
In `analysis_tracking.md`, document:
```markdown
## Execution Log

| Date       | Planned Action | Actual Action | BTC % After | USDT % After | Notes           |
|------------|----------------|---------------|-------------|--------------|------------------|
| Dec 11, 25 | BUY +10%       | BUY +8%       | 68%         | 32%          | Split over 4 days|
```

**Update Portfolio Variables:**
After execution, update for next week:
- **{{CURRENT_BTC_PERCENTAGE}}**: [New BTC %]
- **{{CURRENT_USDT_PERCENTAGE}}**: [New USDT %]
- **{{LAST_ACTION}}**: [What you did]
- **{{LAST_REBALANCE_DATE}}**: [Today's date]

### Step 14: Set Reminder for Next Week

- Add calendar reminder for next Wednesday
- Set alert to check any milestone dates coming up
- Bookmark any new data sources discovered
- Review any price alerts (stop-loss, take-profit levels)

---

## Optional: Advanced Steps

### Visualization (Optional - 15 minutes)
Create or update charts:
- Price prediction timeline
- Probability distribution graph
- Historical prediction accuracy chart
- Key metrics dashboard

Tools: Excel, Google Sheets, Python (matplotlib), TradingView

### Sharing (Optional - 5 minutes)
If sharing publicly:
- Convert to PDF for professional look
- Remove any sensitive personal notes
- Add disclaimer to all shared materials
- Share on Twitter, blog, or with community

### Backtesting (Monthly)
Once per month, review:
- Prediction accuracy over the month
- Which indicators were most reliable
- Calculate error rates (MAPE, RMSE)
- Adjust methodology if needed

---

## Troubleshooting

### Common Issues:

**Issue: Data sources are down or inaccessible**
- Solution: Use alternative sources listed in `analysis_tracking.md`
- Cross-reference multiple sources for critical metrics

**Issue: AI gives inconsistent predictions**
- Solution: Be more specific in prompt, provide more context
- Try running the prompt 2-3 times and compare outputs

**Issue: Major market event disrupts prediction**
- Solution: Run an off-cycle analysis immediately
- Document as "special update" in tracking log
- Adjust base case if invalidation trigger hit

**Issue: Running out of time**
- Solution: Focus on essential metrics only
- Use the most recent previous analysis as template
- Skip optional steps (visualization, sharing)

---

## Checklist Summary

Use this quick checklist each week:

### Pre-Analysis
- [ ] Collect current BTC price and market data
- [ ] Gather on-chain metrics (MVRV, NUPL, exchange flows)
- [ ] Check ETF flows for the week
- [ ] Review macro data (Fed, inflation, DXY)
- [ ] Check sentiment indicators
- [ ] Review last week's analysis
- [ ] Document significant weekly events

### Analysis
- [ ] Update variables in `analysis_tracking.md`
- [ ] Prepare prompt with current context
- [ ] Run analysis through AI assistant
- [ ] Review output for completeness
- [ ] Ask follow-up questions if needed

### Documentation
- [ ] Save analysis as `analysisMMDDYYYY.md`
- [ ] Update prediction history log
- [ ] Update allocation recommendation log
- [ ] Update key events timeline
- [ ] Update milestone checkboxes
- [ ] Fill in week-over-week comparison
- [ ] Check invalidation triggers
- [ ] Document insights and learnings

### Portfolio Management (Optional)
- [ ] Review portfolio recommendation
- [ ] Decide on execution approach
- [ ] Execute rebalancing (if applicable)
- [ ] Record execution in tracking log
- [ ] Update portfolio variables for next week

### Quality Control
- [ ] Sanity check prediction logic
- [ ] Verify data sources
- [ ] Set reminder for next week

---

## File Structure Reference

Your directory should contain:
```
weekly_bitcoin_analysis/
├── prompt.md                    # Main analysis prompt template
├── analysis_tracking.md         # Tracking log and variables
├── weekly_workflow.md          # This file - workflow guide
├── analysis12042025.md         # Week 1 analysis
├── analysis12112025.md         # Week 2 analysis
├── analysis12182025.md         # Week 3 analysis
└── ...                         # Additional weekly analyses
```

---

## Tips for Success

1. **Consistency is key**: Run analysis same day/time each week
2. **Don't skip documentation**: Future you will thank you
3. **Be honest about accuracy**: Track both wins and losses
4. **Iterate and improve**: Update methodology based on learnings
5. **Stay objective**: Don't let emotions influence analysis
6. **Cross-reference sources**: Never rely on single data point
7. **Update promptly**: Market conditions change fast
8. **Backup your files**: Use git or cloud storage

---

## Next Steps

✅ You're ready to run your first weekly analysis!

**For Week 1 (Current Week):**
You already have `analysis04122025.md` completed as your baseline.

**For Week 2 (Next Wednesday):**
1. Follow this workflow from Step 1
2. Use December 4 analysis as your `{{PREVIOUS_PEAK_DATE}}` reference
3. Compare and document changes

**Good luck with your Bitcoin analysis journey!** 🚀

# Run Weekly Bitcoin Analysis - AI Automation Prompt

**Instructions:** Copy this entire file and paste it into your AI assistant (Claude, ChatGPT, etc.) each Wednesday.

---

## Task: Conduct Weekly Bitcoin Analysis with Portfolio Recommendation

You are tasked with conducting a comprehensive weekly Bitcoin market analysis and generating portfolio allocation recommendations. Follow these steps:

### Step 1: Gather Current Market Data

Search the web and collect the following current data:

1. **Bitcoin Price**: Current BTC/USD price
2. **Recent Price Action**: 24h high/low, 7-day performance
3. **Days Post-Halving**: Today's date minus April 20, 2024 (calculate days)
4. **On-Chain Metrics** (use Glassnode, CryptoQuant, or recent reports):
   - MVRV Ratio
   - NUPL (Net Unrealized Profit/Loss)
   - Exchange Whale Ratio (if available)
   - Exchange flows trend (accumulation vs distribution)
5. **ETF Flows**: 
   - Past week's net flows
   - Recent daily flow trends
   - Year-to-date cumulative inflows
6. **Macroeconomic Data**:
   - Current Fed Funds Rate
   - Next FOMC meeting date and rate cut probability
   - Latest CPI or PCE inflation reading
   - USD Index (DXY) level
7. **Sentiment**:
   - Crypto Fear & Greed Index
   - Recent market sentiment trends

### Step 2: Ask User for Portfolio-Specific Variables

After gathering market data, ask the user for the following information:

1. **Current Portfolio Allocation**: 
   - Current BTC percentage
   - Current USDT percentage
2. **Portfolio Value** (optional): Total portfolio value in USD
3. **Last Action Taken**: What was done last week (e.g., "HOLD", "BUY +5%", "SELL -10%")
4. **Last Rebalance Date**: When was the last portfolio adjustment made

Wait for the user's response before proceeding.

### Step 3: Review Previous Week's Analysis

Ask the user:
"Do you have last week's analysis file? If so, please share the key predictions:
- Previous predicted peak date
- Previous predicted peak price
- Previous confidence level

If this is your first analysis after the baseline, use: Sept 15, 2026 at $165K with 55% confidence."

### Step 4: Read the Analysis Prompt Template

Read the file at `/Users/jonasblasques/Dev/AI/weekly_bitcoin_analysis/prompt.md` to understand the full analysis requirements.

### Step 5: Conduct the Analysis

Using all the gathered data, the user's portfolio information, and the prompt template requirements, generate a comprehensive weekly Bitcoin analysis that includes:

1. **Executive Summary** with clear peak prediction
2. **Current Market Status** with all collected data
3. **Detailed Analysis** (halving cycles, on-chain metrics, ETF flows, macro conditions, price projections)
4. **Prediction Breakdown** (Base/Bull/Bear cases with probabilities)
5. **Catalyst and Risk Factors**
6. **What Could Accelerate/Delay the Peak**
7. **What Could Make Price Higher/Lower**
8. **Probability Distribution Table**
9. **Key Levels to Monitor**
10. **Weekly Tracking Metrics**
11. **Portfolio Allocation Recommendation** (BUY/SELL/HOLD with targets, rationale, DCA integration, risk parameters)
12. **Week-Over-Week Comparison** (if not first analysis)

### Step 6: Format the Output

Structure the analysis with:
- Clear markdown formatting
- Proper headings and sections
- Tables for probability distributions
- Bold text for key information
- Professional, shareable format

### Step 7: Update Tracking Document (AUTOMATIC)

**IMPORTANT: This step must be performed automatically by the AI. Do NOT ask the user to manually update the tracking file.**

After completing the analysis:

1. **Read** the tracking file: `analysis_tracking.md`
2. **Automatically update** the following sections using the Edit tool:
   - **Current Variables Section**: Update with new week's values
   - **Prediction History Log**: Add new table row
   - **Allocation Recommendation Log**: Add new table row
   - **Execution Log**: Add new table row
   - **Key Events Timeline**: Add significant events from this week
   - **Weekly Milestones**: Update checkboxes (mark completed items with [x])
   - **Week-Over-Week Changes Log**: Fill in the current week's section with changes and new data
   - **Final Prediction Assessment**: Update target peak information

3. **Confirm** to the user that tracking updates have been applied automatically

### Step 8: Save the Analysis

Save the analysis automatically as `analysisDDMMYYYY.md` using the Write tool with today's date (format: DD=day, MM=month, YYYY=year).

---

## Summary of What YOU (AI) Will Do:
✅ Search web for current Bitcoin price, on-chain data, ETF flows, macro data, sentiment
✅ Calculate days post-halving
✅ Ask user for portfolio-specific variables
✅ Ask user for previous week's predictions
✅ Read prompt template to understand requirements
✅ Generate complete analysis with portfolio recommendation
✅ **AUTOMATICALLY update `analysis_tracking.md` using Edit tool (DO NOT ask user to do this manually)**
✅ **AUTOMATICALLY save analysis as `analysisDDMMYYYY.md` using Write tool (DD=day, MM=month, YYYY=year)**
✅ Confirm completion to user

## Summary of What USER Will Do:
✅ Paste this prompt into AI
✅ Provide portfolio allocation percentages and last action
✅ Provide previous week's prediction (if available)
✅ Review the completed analysis
✅ (Optional) Execute portfolio recommendation  

---

**Ready? Start by gathering the current market data now.**

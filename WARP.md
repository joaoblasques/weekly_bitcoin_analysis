# WARP.md

This file provides guidance to WARP (warp.dev) when working with code in this repository.

## Repository Overview

This is a personal Bitcoin market analysis framework for conducting weekly peak predictions and portfolio allocation recommendations. The system uses AI-assisted analysis combining on-chain metrics, ETF flows, macroeconomic data, and sentiment indicators.

**Key Concept**: This is NOT a codebase—it's a structured documentation system for tracking Bitcoin market predictions and portfolio decisions over time.

## Core Architecture

### Primary Workflow (Automated)
1. User copies `run_weekly_analysis.md` into an AI assistant (Claude, ChatGPT, Gemini)
2. AI gathers current market data via web search
3. AI reads `prompt.md` template for analysis requirements
4. AI generates complete analysis with portfolio recommendations
5. User saves output as `analysisMMDDYYYY.md` and updates `analysis_tracking.md`

### Secondary Workflow (Manual)
1. User manually gathers market data
2. User updates variables in `analysis_tracking.md`
3. User runs AI analysis with `prompt.md` template
4. User saves and documents results

### File Structure
```
run_weekly_analysis.md    → Automated AI workflow (copy/paste to AI)
prompt.md                 → Analysis template and requirements
analysis_tracking.md      → Variables, logs, and milestones
weekly_workflow.md        → Manual step-by-step guide
analysisMMDDYYYY.md      → Weekly analysis outputs (dated)
README.md                 → System documentation
QUICK_START.md           → Quick reference guide
```

## Common Commands

### View Current Analysis Variables
```bash
head -25 analysis_tracking.md
```

### List All Past Analyses
```bash
ls -lt analysis*.md
```

### View Latest Analysis
```bash
ls -t analysis*.md | head -1 | xargs cat
```

### Search for Specific Predictions
```bash
grep -E "Peak Date|Peak Price|Confidence" analysis*.md
```

### Check Tracking Logs
```bash
grep -A 10 "Prediction History Log" analysis_tracking.md
grep -A 10 "Allocation Recommendation Log" analysis_tracking.md
```

## Key System Concepts

### Variable Substitution Pattern
Files use `{{VARIABLE_NAME}}` placeholders that should be replaced with current values:
- `{{CURRENT_DATE}}` - Today's date
- `{{CURRENT_PRICE}}` - Current BTC price
- `{{DAYS_POST_HALVING}}` - Days since April 20, 2024
- `{{CURRENT_BTC_PERCENTAGE}}` - Current BTC allocation %
- `{{CURRENT_USDT_PERCENTAGE}}` - Current USDT allocation %
- `{{PREVIOUS_PEAK_DATE}}` - Last week's predicted peak date
- `{{PREVIOUS_PEAK_PRICE}}` - Last week's predicted peak price

### Halving Date Reference
The Bitcoin halving occurred on **April 20, 2024**. All "days post-halving" calculations reference this date.

### File Naming Convention
Weekly analyses use format: `analysisMMDDYYYY.md`
- `MM` = 2-digit month
- `DD` = 2-digit day  
- `YYYY` = 4-digit year
- Example: `analysis12042025.md` for December 4, 2025

### Portfolio Allocation Framework
- **Two-asset portfolio**: BTC and USDT only
- **Min BTC allocation**: 10% (never full cash)
- **Max BTC allocation**: 90% (always keep dry powder)
- **Actions**: BUY (increase BTC %), SELL (decrease BTC %), HOLD, DCA ONLY
- **Base DCA**: Consistent periodic purchases (default: 5%/month)

## Working with Analysis Files

### Creating a New Weekly Analysis
The recommended approach is to use the automated workflow:

1. Copy entire contents of `run_weekly_analysis.md`
2. Paste into AI assistant
3. Provide portfolio information when prompted
4. Save AI output as new dated analysis file

### Updating Tracking Logs
After generating an analysis, update `analysis_tracking.md`:

**Current Variables** (top of file):
- Update market data (date, price, days post-halving)
- Update portfolio allocation percentages
- Update last action and rebalance date

**Prediction History Log** (table):
- Add new row with: week date | predicted peak date | predicted price | confidence | status | notes

**Allocation Recommendation Log** (table):
- Add new row with: week date | action | target BTC % | target USDT % | rationale

**Week-Over-Week Changes Log**:
- Document prediction changes
- List new data that influenced changes
- Record key events from the week

### Reading Previous Analyses
All past analyses are preserved as dated markdown files. To reference:
```bash
cat analysis12042025.md  # View specific week
```

## Data Sources Used

### On-Chain Metrics
- MVRV Ratio (Market Value to Realized Value)
- NUPL (Net Unrealized Profit/Loss)
- Exchange Whale Ratio
- Exchange flows (accumulation vs distribution)
- Long/short-term holder behavior

### Market Data
- BTC/USD price (CoinMarketCap, CoinGecko, TradingView)
- ETF flows (SoSoValue, Bloomberg)
- Trading volume and open interest

### Macroeconomic Data
- Federal Reserve policy (Fed Funds Rate, FOMC decisions)
- Inflation data (CPI, PCE)
- USD Index (DXY)
- Global liquidity (M2)

### Sentiment Indicators
- Fear & Greed Index (Alternative.me)
- Social media sentiment (LunarCrush)
- Google Trends (Bitcoin search interest)

## Important Context for AI Assistants

When working with this repository:

1. **Python Command**: Use `python3` (aliased from `python`)

2. **File Reading**: Always read `prompt.md` to understand analysis requirements before generating output

3. **Web Search Needed**: Current market data must be gathered via web search—values change weekly

4. **No Code Execution**: This system doesn't require running Python scripts or programs; it's purely documentation-based

5. **Markdown Format**: All outputs should be well-formatted markdown with tables, headings, and bullet points

6. **Preserve History**: Never overwrite existing `analysisMMDDYYYY.md` files—each week creates a new dated file

7. **Scenario Analysis Required**: All predictions must include Base/Bull/Bear cases with probabilities

8. **Portfolio Recommendations**: Every analysis should include actionable BUY/SELL/HOLD guidance with rationale

## Tracking & Accountability System

### Three Core Logs

**Prediction History Log**
- Tracks weekly peak date and price predictions
- Includes confidence levels
- Enables accuracy assessment over time

**Allocation Recommendation Log**
- Records weekly portfolio actions (BUY/SELL/HOLD)
- Documents target allocations and rationale
- Shows strategy evolution

**Execution Log**
- Records actual trades made (if any)
- Compares planned vs actual actions
- Tracks portfolio performance

### Accuracy Metrics
When milestones are reached:
- Compare predicted dates/prices to actual outcomes
- Calculate error rates (date error %, price error %)
- Document which indicators were most/least reliable
- Adjust methodology based on learnings

## Tips for Productive Analysis

### Before Generating New Analysis
1. Check last week's prediction in `analysis_tracking.md`
2. Review any milestone checkboxes that may have been completed
3. Note significant market events from the past 7 days

### When AI Can't Access Web Search
Provide manual inputs:
- Current BTC price from CoinMarketCap
- Recent on-chain metrics from Glassnode/CryptoQuant
- Latest Fed policy updates
- Recent ETF flow data from SoSoValue

### Quality Checks
- Probabilities should sum to ~100% across Base/Bull/Bear cases
- MVRV and NUPL values should be realistic (MVRV: 1-4, NUPL: 0-1)
- Days post-halving should be calculated from April 20, 2024
- Portfolio allocation percentages should add to 100%

### Consistency Principles
- Run analysis same day each week (recommended: Wednesdays)
- Use consistent data sources week-over-week
- Document all significant changes in week-over-week comparison
- Never skip updating tracking logs

## Customization Options

Users can adjust system parameters in `prompt.md`:

**DCA Rate**: Change base DCA percentage (default: 5%/month)
```markdown
- Base DCA: Consistent weekly/monthly BTC purchase size (e.g., 2-5%/month)
```

**Allocation Guardrails**: Modify min/max BTC limits (default: 10-90%)
```markdown
- Guardrails: Min BTC 10%, Max BTC 90% unless explicitly justified
```

**Rebalancing Frequency**: Adjust cadence (default: weekly)
```markdown
- Rebalancing cadence: Weekly by default; allow event-driven adjustments
```

## Disclaimers

This system is for informational and educational purposes only. It does NOT constitute financial, investment, or trading advice. Bitcoin is highly volatile and can result in significant losses. Users are solely responsible for their investment decisions.

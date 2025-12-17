# Weekly Bitcoin Analysis & Portfolio Management System

A comprehensive framework for conducting weekly Bitcoin market peak predictions and generating data-driven portfolio allocation recommendations.

---

## 🎯 System Overview

This system combines:
1. **Market Peak Prediction** - Forecast BTC cycle top date and price
2. **Portfolio Allocation** - Tactical BTC/USDT rebalancing recommendations
3. **DCA Integration** - Systematic accumulation with intelligent overlays
4. **Historical Tracking** - Monitor accuracy and refine methodology

---

## 📁 File Structure

```
weekly_bitcoin_analysis/
├── README.md                    # This file - system overview
├── run_weekly_analysis.md       # 🚀 START HERE - Automated AI workflow (paste into AI)
├── prompt.md                    # AI prompt template reference (for advanced users)
├── analysis_tracking.md         # Variables, logs, and milestones (you update this)
├── weekly_workflow.md           # Manual step-by-step guide (alternative to automation)
├── analysis04122025.md          # Weekly analysis outputs (dated, format: DDMMYYYY)
└── ...                          # Additional weekly analyses
```

---

## 🔑 Key Features

### 1. Market Analysis
- **Cycle-based prediction** using halving patterns
- **On-chain metrics** (MVRV, NUPL, exchange flows)
- **ETF flow tracking** and institutional behavior
- **Macro context** (Fed policy, inflation, USD)
- **Scenario modeling** (Base/Bull/Bear cases with probabilities)

### 2. Portfolio Allocation Recommendations

**New Feature:** Each weekly analysis now includes actionable portfolio guidance.

#### Portfolio Context
- **Two-asset portfolio**: BTC and USDT only
- **Strategy**: Dollar-Cost Averaging (DCA) with tactical overlays
- **Actions**: BUY (increase BTC %), SELL (decrease BTC %), HOLD, or DCA ONLY

#### Recommendation Components
- **Target Allocation**: Specific BTC % and USDT % targets
- **Rationale**: Data-driven justification using cycle position, on-chain signals, macro backdrop
- **DCA Integration**: Base DCA rate (e.g., 5%/month) + tactical tilts (e.g., +10% this week)
- **Risk Parameters**: Stop-loss triggers, take-profit zones, rebalancing guardrails

#### Example Output
```
RECOMMENDED ACTION: BUY +10% BTC
Target Allocation: 70% BTC / 30% USDT (from 60/40)
Rationale: Mid-cycle consolidation, MVRV 1.8, supportive ETF flows, 
           ~9 months to projected peak. Risk/reward favorable.
DCA: Maintain 5% monthly base DCA; add one-time +10% tilt this week.
Risk: If < $80K reduce to 50%; > $120K trim to 60%; > $150K trim to 40%.
```

#### Guardrails
- **Min BTC allocation**: 10% (never full cash)
- **Max BTC allocation**: 90% (always keep dry powder)
- **Base DCA continues**: Consistent weekly/monthly purchases regardless of tactical overlays
- **Weekly rebalancing**: Default cadence with event-driven adjustments allowed

---

## 🚀 Quick Start

> **👉 BRAND NEW? Read [`START_HERE.md`](START_HERE.md) first - it's a 2-minute guide!**

### What This System Does

This is an **AI-automated Bitcoin analysis system**:
- **You:** Copy one file (`run_weekly_analysis.md`) into an AI assistant weekly
- **AI:** Gathers all data, generates analysis, updates tracking, saves everything
- **Time:** 10-15 minutes per week
- **Result:** Complete market analysis + portfolio recommendations

### First-Time Setup (5 minutes)

1. **Read the quick start guide**:
   - Open **[`START_HERE.md`](START_HERE.md)** ← Your main onboarding guide
   - Understand the 4-step weekly workflow
   - Set up your Wednesday calendar reminder

2. **Your baseline analysis is complete**: You have 3 weeks of data (Dec 4, 10, 17)

3. **You're ready to run weekly analyses!**

### Weekly Execution (10 minutes - Fully Automated)

Every Wednesday:

1. **Open** `run_weekly_analysis.md`
2. **Copy & paste** entire file into AI assistant (Claude, ChatGPT, Gemini)
3. **Answer** AI's questions:
   - Current portfolio allocation (e.g., "36% BTC, 64% USDT")
   - Last action taken (e.g., "DCA buy 1.25%")
   - Current BTC price (if AI can't fetch it)
4. **Done!** AI automatically:
   - ✅ Gathers all market data
   - ✅ Generates complete analysis
   - ✅ Updates `analysis_tracking.md`
   - ✅ Saves `analysisDDMMYYYY.md`
   - ✅ Provides portfolio recommendation

**That's it!** The entire process takes 10 minutes.

---

## 📁 File Structure (Simplified)

```
weekly_bitcoin_analysis/
├── START_HERE.md                ← 🚀 READ THIS FIRST! (2-min quick start)
├── run_weekly_analysis.md       ← Your main file (copy/paste weekly)
├── analysis_tracking.md         ← Auto-updated by AI (view history)
├── prompt.md                    ← Backend (AI reads this, you don't touch)
├── README.md                    ← This file (full documentation)
├── WARP.md                      ← Repository guidance
├── analysis04122025.md          ← Week 1 (04 Dec 2025)
├── analysis10122025.md          ← Week 2 (10 Dec 2025)
├── analysis17122025.md          ← Week 3 (17 Dec 2025 - latest)
└── archive/
    └── weekly_workflow.md       ← Manual process (advanced users only)
```

---

## 🎯 Which File Do I Use?

| File | When to Use | Who It's For | Action |
|------|-------------|--------------|--------|
| **[START_HERE.md](START_HERE.md)** | First time | Everyone | **Read this first!** (2 min) |
| **run_weekly_analysis.md** | Every Wednesday | Everyone | Copy/paste to AI |
| **analysis_tracking.md** | View history | Everyone | Just review (auto-updated) |
| **README.md** | Need details | Reference | This file - full docs |
| **prompt.md** | Never | AI only | Don't touch (backend) |
| **archive/** | Optional | Advanced | Ignore (old files) |

---

## 🤖 How It Works (Behind the Scenes)

```
You → Copy run_weekly_analysis.md
        ↓
    Paste into AI
        ↓
    AI reads prompt.md (automatically)
        ↓
    AI gathers market data
        ↓
    AI generates analysis
        ↓
    AI updates tracking files
        ↓
    Done!
```

You never need to touch `prompt.md` - it's the "instruction manual" the AI reads automatically.

---

## 📊 Portfolio Management Philosophy

### Dollar-Cost Averaging (DCA) Foundation
- **Base strategy**: Consistent periodic BTC purchases (e.g., 5% of portfolio monthly)
- **Emotional discipline**: Removes timing decisions during high volatility
- **Long-term accumulation**: Builds position regardless of short-term price

### Tactical Overlays
- **Data-driven tilts**: Temporary allocation adjustments based on analysis
- **Cycle-aware**: Increase exposure early/mid-cycle, reduce exposure near peaks
- **Signal-based**: Use on-chain metrics, ETF flows, macro context to inform tilts
- **Reversible**: Tactical changes complement but don't replace base DCA

### Risk Management
- **Position sizing**: Never all-in, never all-out
- **Stop-loss levels**: Pre-defined price levels to reduce exposure
- **Take-profit zones**: Scale down BTC as price approaches targets
- **Flexibility**: Allow manual override if conditions change rapidly

---

## 📈 How Recommendations Are Generated

The AI analyzes multiple factors to suggest portfolio adjustments:

### 1. Cycle Position
- Days post-halving vs historical peak timing
- Time remaining to predicted peak
- Early cycle = more aggressive, late cycle = more conservative

### 2. Valuation Metrics
- MVRV ratio (overheated vs undervalued)
- NUPL (euphoria vs fear)
- Current price vs predicted peak price

### 3. Momentum Indicators
- ETF flows (institutional demand)
- Exchange flows (accumulation vs distribution)
- On-chain activity (long-term holder behavior)

### 4. Macro Context
- Fed policy direction (easing = bullish, tightening = bearish)
- Inflation trends, USD strength
- Risk-on vs risk-off environment

### 5. Technical Levels
- Key support/resistance levels
- Trend confirmation/invalidation

---

## 📋 Tracking & Accountability

### Three Key Logs

1. **Prediction History Log**
   - Tracks weekly predictions (date, price, confidence)
   - Enables accuracy assessment over time

2. **Allocation Recommendation Log**
   - Records weekly recommendations (action, targets, rationale)
   - Documents portfolio strategy evolution

3. **Execution Log**
   - Records actual portfolio changes made
   - Tracks planned vs actual actions
   - Enables performance analysis

### Accuracy Tracking
- Compare predictions to reality as milestones pass
- Calculate error rates (date error, price error)
- Adjust methodology based on learnings
- Document which indicators were most/least reliable

---

## ⚙️ Customization Options

### Adjust Your DCA Rate
In `prompt.md`, modify the base DCA rate:
```markdown
- Base DCA: Consistent weekly/monthly BTC purchase size (e.g., 2-5%/month)
```
Change to your preferred rate (e.g., 10%/month for aggressive, 2%/month for conservative)

### Modify Allocation Guardrails
In `prompt.md`, adjust min/max limits:
```markdown
- Guardrails: Min BTC 10%, Max BTC 90% unless explicitly justified
```
Change to your risk tolerance (e.g., 20%-80% for more conservative)

### Change Rebalancing Frequency
Default is weekly. You can:
- Run analysis weekly but only rebalance monthly
- Set up event-driven triggers (e.g., only rebalance on >10% moves)
- Adjust in `prompt.md` under "Rebalancing cadence"

### Portfolio Size
The system works with percentage allocations, so it's size-agnostic. Whether you have $1K or $1M, the recommendations are based on % of portfolio.

---

## 💡 Usage Tips

### For Beginners
1. **Start with DCA only**: Ignore tactical recommendations for first month
2. **Small adjustments**: Limit tactical overlays to ±5% initially
3. **Focus on learning**: Track predictions without executing to build confidence
4. **Conservative guardrails**: Use tighter min/max bounds (e.g., 30%-70%)

### For Intermediate Users
1. **Follow base case recommendations**: Execute suggested actions with standard sizes
2. **Split execution**: Use time-weighted execution to reduce timing risk
3. **Track performance**: Compare your results to pure DCA and pure HODL
4. **Refine methodology**: Adjust based on what's working

### For Advanced Users
1. **Integrate other signals**: Add your own analysis to the recommendation
2. **Use limit orders**: Execute at better prices within recommendation range
3. **Size tactically**: Vary adjustment size based on conviction
4. **Automate**: Consider programmatic execution for discipline

---

## ⚠️ Important Disclaimers

1. **Not Financial Advice**: This system is for informational and educational purposes only. It does not constitute financial, investment, or trading advice.

2. **No Guarantees**: Past performance does not predict future results. Bitcoin is highly volatile and can result in significant losses.

3. **Personal Responsibility**: You are solely responsible for your investment decisions. Always do your own research and never invest more than you can afford to lose.

4. **AI Limitations**: AI analysis is based on historical patterns and current data, but cannot predict black swan events, regulatory changes, or other unforeseen circumstances.

5. **Risk Disclosure**: Cryptocurrency investments carry substantial risk, including the possibility of total loss of capital.

---

## 🔄 System Updates

### Version History
- **v1.0** (Dec 4, 2025): Initial system with market prediction
- **v1.1** (Dec 4, 2025): Added portfolio allocation recommendations and DCA integration

### Future Enhancements
Potential additions to consider:
- [ ] Automated data collection scripts
- [ ] Visualization dashboard for predictions and portfolio
- [ ] Backtesting framework for historical accuracy
- [ ] Integration with exchange APIs for execution
- [ ] Multi-asset expansion (BTC, ETH, USDT)
- [ ] Risk-adjusted performance metrics (Sharpe ratio, max drawdown)

---

## 📞 Support & Community

This is a personal framework. Adapt it to your needs:
- Modify prompts to match your investment style
- Adjust guardrails for your risk tolerance
- Add/remove metrics based on what you trust
- Share learnings and improvements with community

---

## 🎓 Resources

### Data Sources Used
- **On-chain**: Glassnode, CryptoQuant, IntoTheBlock
- **Market**: CoinMarketCap, CoinGecko, TradingView
- **ETF Flows**: SoSoValue, Bloomberg
- **Macro**: Federal Reserve, CME FedWatch, BLS
- **Sentiment**: Alternative.me, LunarCrush, Google Trends

### Learning Materials
- Study historical Bitcoin halving cycles
- Understand on-chain metrics (MVRV, NUPL, etc.)
- Learn DCA principles and behavioral finance
- Follow Bitcoin macro analysts and researchers

---

## 📝 Quick Reference

### Automated Weekly Checklist (Recommended)
1. ✅ Open `run_weekly_analysis.md`
2. ✅ Copy & paste into AI assistant
3. ✅ Answer AI's questions (portfolio allocation, last action)
4. ✅ Review AI's complete analysis
5. ✅ Copy tracking updates to `analysis_tracking.md`
6. ✅ Save analysis as `analysisDDMMYYYY.md`
7. ✅ (Optional) Execute portfolio recommendation

### Manual Weekly Checklist (Alternative)
1. ✅ Gather current market data
2. ✅ Update variables in tracking document
3. ✅ Run AI analysis with prompt
4. ✅ Review prediction and allocation recommendation
5. ✅ Save analysis with date-stamped filename
6. ✅ Update logs (prediction, allocation, execution)
7. ✅ Execute portfolio rebalancing (optional)
8. ✅ Quality check and set reminders

### Key Files Quick Access
- **🚀 NEW? START HERE**: **[`START_HERE.md`](START_HERE.md)** ← Read this first! (2-minute guide)
- **📋 Weekly Analysis**: `run_weekly_analysis.md` (copy/paste to AI every Wednesday)
- **📊 View History**: `analysis_tracking.md` (auto-updated by AI)
- **📖 Full Docs**: `README.md` (this file)
- **⚙️ Backend**: `prompt.md` (don't touch - AI uses this)
- **📦 Archive**: `archive/weekly_workflow.md` (manual process - skip unless you want full control)

---

---

## 🎉 You're All Set!

**Next Wednesday (December 24, 2025):**
1. Open `run_weekly_analysis.md`
2. Copy entire file (Cmd+A, Cmd+C)
3. Paste into AI assistant
4. Answer 3 questions
5. Done in 10 minutes!

**💡 Pro Tip:** Set a weekly calendar reminder for every Wednesday at 10am with the title "Bitcoin Analysis - Copy run_weekly_analysis.md"

---

## 📚 Additional Resources

- **[START_HERE.md](START_HERE.md)** - 2-minute quick start guide (read this first!)
- **WARP.md** - Repository guidance for developers and AI assistants
- **archive/** - Old manual workflows (advanced users only)

---

**The AI handles everything. You just copy/paste weekly. Simple!** 🚀

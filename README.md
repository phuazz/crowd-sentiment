# US Crowd Sentiment Composite

**Live: https://phuazz.github.io/crowd-sentiment/**

A daily crowd-sentiment state for the S&P 500 built from 11 live
inputs — a survey (AAII), positioning (CFTC COT), options (put/call,
SKEW), breadth and volume, credit vs earnings yield — each scored against
adaptive extreme bands fitted to its own trailing history. The composite is
the share of components at bullish extremes (half-credit for neutral),
used as a proxy for investor sentiment. NAAIM, one of the original
12 inputs, retired in August 2026 and contributes only to the historical record.

The landing tab shows the weekly S&P 500 overlay. The 21-session average
sets the target addition to the base portfolio at 0% for readings of
41.5 or above, +30% from 30 to below 41.5 and +60% below 30. The
second-last NYSE session of the week supplies the reading for the
following week’s first close. The chart and decision history show
targets before the breadth-based 150% cap. The public proxy can trigger
on different dates from the strategy’s original input.

The price chart and forward-return panels distinguish Pessimism from Deep
pessimism using the weekly review band. Index price returns run from the
model fill close to the close 5, 21, 63, 126 or 252 sessions later.
Each table cell gives its eligible review count. Consecutive weekly
reviews can have overlapping forward windows.

The dashboard also retains the separate five-day signal and its research:

- **State conditioner, not an entry trigger** — zone-entry timing fails
  random-entry nulls; the one significant trigger (fresh drop below 25) is
  shown with cluster-preserving p-values.
- **A costed tilt overlay was tested under a pre-registered rule and
  REJECTED** — published on the page as a negative result.
- Extended-bear absolute losses, overlapping-window caveats and the
  no-untouched-holdout status of the display smoothing are all disclosed.

Data: public feeds (AAII, CFTC, OFR, Yahoo Finance) plus licensed
end-of-day market data (Norgate) — only derived scores and statistics are
published, never vendor series values. Survey and positioning series enter
at their public release dates. The dashboard displays the most recent
observation date alongside the model review and fill dates.

This repository hosts the built page only; the research engine is private.
Educational content — not investment advice.

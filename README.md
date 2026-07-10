# US Crowd Sentiment Composite

**Live: https://phuazz.github.io/crowd-sentiment/**

A daily crowd-sentiment state for the S&P 500 built from 12 public-sourced
inputs — surveys (AAII, NAAIM), positioning (CFTC COT), options (put/call,
SKEW), breadth and volume, credit vs earnings yield — each scored against
adaptive extreme bands fitted to its own trailing history. The composite is
the share of components at bullish extremes (half-credit for neutral),
read contrarian: hold more equity while the crowd is depressed, trim when
it is euphoric and financial conditions are tight.

Highlights of the honesty-first design:

- **State conditioner, not an entry trigger** — zone-entry timing fails
  random-entry nulls; the one significant trigger (fresh drop below 25) is
  shown with cluster-preserving p-values.
- **A costed tilt overlay was tested under a pre-registered rule and
  REJECTED** — published on the page as a negative result.
- Extended-bear absolute losses, overlapping-window caveats and the
  no-untouched-holdout status of the display smoothing are all disclosed.

Data: public feeds (AAII, NAAIM, CFTC, OFR, Yahoo Finance) plus licensed
end-of-day market data (Norgate) — only derived scores and statistics are
published, never vendor series values. Survey and positioning series enter
at their public release dates. Updated weekly (Saturdays SGT).

This repository hosts the built page only; the research engine is private.
Educational content — not investment advice.

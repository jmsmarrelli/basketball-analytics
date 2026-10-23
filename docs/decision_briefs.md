# From a finding to a basketball decision

Five proposed staff workflows based on the flagship studies. AI-assisted synthesis, October 22, 2026. No completed film review, causal coaching effect or NBA-team deployment is claimed.

## when to change the shooting scout

AI-assisted synthesis of the existing study, October 22, 2026. This is a proposed staff workflow, not a report of work performed for an NBA team. No film was reviewed for this brief.

**Decision:** use the January forecast to prioritize a shooting review, while retaining the prior-history estimate as the principal comparison. A hot raw percentage alone is weak evidence for a new coverage rule.

![Prior forecasts, updated probabilities and early observed rates with uncertainty](https://github.com/jmsmarrelli/basketball-research/blob/main/figures/shooter_updates.png)

**Evidence:** the updated forecast improves held-out log loss by 0.00402 relative to the early percentage, but only 0.00019 relative to prior history alone. The latter 95% player-bootstrap interval is −0.000342 to −0.000040. There are 46,184 later attempts from 312 evaluated players; three forecasted players have no later attempts. These numbers support a modest predictive improvement in this backtest, not an estimate of points saved by a defensive scheme.

**Proposed next step:** review players with meaningful changes in both the forecast and their opportunity mix. Check corner share, catch-and-shoot versus pull-up opportunities where legitimately available, and whether the offensive role has changed. The public table already supports a corner-share check; the other tags require additional data or actual film coding. Select a review rule before looking at subsequent shooting results, and compare its usefulness against reviewing the highest-volume players.

**What would change the recommendation:** failure to improve on prior history in a new locked chronological backtest, subgroup miscalibration, or systematic role changes that make the historical prior inappropriate. A posterior interval for latent skill does not describe the full range of a player's percentage over the next ten attempts.

**Interview defense:** explain the distinction between an empirical prior, a player-history update and a forecast evaluated on later attempts. The ten largest movers in the chart illustrate shrinkage; selecting those movers after observing early results does not create a representative performance sample.

Sources: [full study](https://github.com/jmsmarrelli/basketball-research/blob/main/reports/03_when_to_update_a_shooter.md), [forecast table](https://github.com/jmsmarrelli/basketball-research/blob/main/results/shooter_forecasts.csv), [backtest summary](https://github.com/jmsmarrelli/basketball-research/blob/main/results/shooter_summary.json), and [execution limits](https://github.com/jmsmarrelli/basketball-research/blob/main/VALIDATION_CURRENT.md).


---

## separate rim access from rim finishing

AI-assisted synthesis of the existing study, October 22, 2026. The review protocol below is proposed; no film review or team deployment is claimed.

**Decision:** organize the Wembanyama review around how opponents reach the rim, then examine finishing conditional on getting there. Combining those questions into one field-goal percentage conceals the more precise finding.

![Adjusted rim-access and finishing comparisons with game-bootstrap intervals](https://github.com/jmsmarrelli/spurs-research/blob/main/figures/rim_adjusted.png)

**Evidence:** across 63 games with observations in both on/off states, adjusted rim-attempt share is 4.6 percentage points lower during his minutes; the 95% interval is −7.0 to −2.3. The corresponding finishing estimate is −0.7 points with an interval from −5.7 to +4.2. The finishing interval is compatible with several meaningful effects; it does not prove there is no finishing effect. The denominators differ: 5,726 total opponent attempts versus 1,436 rim attempts.

**Proposed next step:** sample both successful rim entries and possessions ending elsewhere, stratified by his on/off state and game. A rim-attempt-only queue cannot show successful deterrence. Have reviewers record the initial action, help location, screening involvement, entry route and whether the possession was transition or settled offense. Include an explicit unobservable category rather than inferring a responsibility from the result.

**What would change the recommendation:** failure of the lineup audit, sensitivity to a few games, or substantial changes after accounting for role and teammate/opponent combinations. Conditioning on attempted shots can hide changes in turnovers, fouls and possessions without a field-goal attempt. The existing study cannot account for those channels as a complete defensive value model.

**Interview defense:** game fixed effects remove shared game-level differences, not lineup selection within a game. The bootstrap resamples games because attempts from the same game are dependent. A full raw-source rebuild remains blocked by omitted source files; the estimates were verified from committed model rows.

Sources: [full study](https://github.com/jmsmarrelli/spurs-research/blob/main/reports/01_wembanyama_rim_footprint.md), [estimates](https://github.com/jmsmarrelli/spurs-research/blob/main/results/rim_estimates.csv), [sensitivity results](https://github.com/jmsmarrelli/spurs-research/blob/main/results/rim_sensitivity.csv), and [execution limits](https://github.com/jmsmarrelli/spurs-research/blob/main/VALIDATION_CURRENT.md).


---

## turn turnover counts into a review priority

AI-assisted synthesis of the existing study, October 22, 2026. The proposed review and intervention have not been carried out.

**Decision:** prioritize the first defensive actions after steal-linked losses in the ball-security review. Do not turn the estimated scoring gap directly into a promised coaching benefit.

![Adjusted 12-second scoring gaps across three overlapping samples](https://github.com/jmsmarrelli/spurs-game-management/blob/main/figures/turnover_adjusted.png)

**Evidence:** the main within-game comparison is +0.69 opponent points over the next 12 game-clock seconds after steal-linked versus other turnovers, with a 95% interval of +0.58 to +0.79. It covers 1,007 turnovers in 79 games: 582 steal-linked and 425 others. Estimates remain positive under the reported score/clock and timeout restrictions. The restricted samples overlap the main sample, so their agreement is a sensitivity check rather than independent replication.

**Proposed next step:** use the existing event queue to code the turnover mechanism, location, number of defenders behind the ball and first recovery assignment. Include comparable non-steal losses. Treat missing linkage and ambiguous event ordering explicitly. Counts by player need an opportunity denominator before becoming player rankings; touches and passing exposure are not interchangeable with minutes.

**What would change the recommendation:** widespread errors in steal linkage, a materially different result under alternate event-order rules, or evidence that the selected review queue misses damaging non-steal live-ball losses. Outcomes at 8, 12 and 16 seconds are related measurements, not separate independent experiments.

**A prospective evaluation:** define one coaching cue and a fixed evaluation period before implementation. Track a process measure such as recovery-assignment execution alongside points allowed, annotate personnel and opponent changes, and compare with a predeclared baseline. Without a credible comparison, describe the results as a monitored pilot rather than a causal intervention estimate.

Sources: [full study](https://github.com/jmsmarrelli/spurs-game-management/blob/main/reports/01_turnover_cost.md), [adjusted results](https://github.com/jmsmarrelli/spurs-game-management/blob/main/results/turnover_adjusted.csv), [review queue](https://github.com/jmsmarrelli/spurs-game-management/blob/main/results/turnover_review_queue.csv), and [execution limits](https://github.com/jmsmarrelli/spurs-game-management/blob/main/VALIDATION_CURRENT.md).


---

## make the rebounding plan opponent-specific

AI-assisted synthesis of the existing study, October 22, 2026. This proposes a scouting review; it does not claim completed film coding or an implemented game plan.

**Decision:** allocate the first rebounding review block to Houston. Investigate the mechanism before prescribing which players should stay home or release.

![Western opponents compared with shot-context expectations and uncertainty](https://github.com/jmsmarrelli/west-playoff-scouting/blob/main/figures/glass_adjusted.png)

**Evidence:** Houston recovers 34.1% of eligible player-rebound chances against a shot-context expectation of 26.9%. Its league-relative residual is +7.6 percentage points, with a 95% interval of +5.6 to +9.6, from 2,048 chances in 50 later-sample games. The 7.6-point figure is not simply 34.1 minus 26.9: it also subtracts the later league's −0.42-point residual. The chronological rebound model improves log loss from 0.57926 to 0.57401 on 59,658 later chances.

**Proposed next step:** stratify Houston misses by shot location and lineup, then code first contact, weak-side position, rebound trajectory and transition release responsibility. Review matched examples with and without an offensive rebound. Use the recorded rebounder counts to find examples, not to claim opportunity-adjusted individual skill. Refresh personnel before operational use; this is a 2025–26 study.

**What would change the recommendation:** a materially different result once team/dead-ball rebounds are accounted for, failure to transfer to a later season, or film showing that the apparent team effect is concentrated in a narrow personnel configuration. Player positioning and box-outs are absent from these data.

**Companion map:** the [OKC shot geography study](https://github.com/jmsmarrelli/west-playoff-scouting/blob/main/reports/02_okc_shot_map.md) offers another review question. Its colors show differences in attempt frequency per 100 total field-goal attempts; they do not show defensive pressure, openness or shot value. Keep location and conversion claims separate.

Sources: [full rebounding study](https://github.com/jmsmarrelli/west-playoff-scouting/blob/main/reports/03_western_glass.md), [team results](https://github.com/jmsmarrelli/west-playoff-scouting/blob/main/results/glass_profiles.csv), [validation](https://github.com/jmsmarrelli/west-playoff-scouting/blob/main/results/glass_validation.json), and [execution limits](https://github.com/jmsmarrelli/west-playoff-scouting/blob/main/VALIDATION_CURRENT.md).


---

## use expected points as a reference, not a verdict

AI-assisted synthesis of Project 05, October 22, 2026. Recommendations below are proposed uses, not claims of deployment by a team.

**Decision:** use the recorded-context model to separate a description of the shot diet from conversion. Keep a zone-only baseline in every model review and avoid treating actual-minus-expected as isolated shooting skill.

![Held-out calibration and log-loss comparison for the shot-context model](https://github.com/jmsmarrelli/nba-analytics-portfolio/blob/main/projects/05_shot_quality/figures/calibration.png)

**Evidence:** on 219,160 held-out 2025–26 attempts, log loss is 0.63661 versus 0.65723 for the zone baseline, a 3.1% relative reduction in this loss metric. Brier score is 0.22386 versus 0.23227. Training covers 1,251,267 earlier-season attempts. San Antonio's expected field-goal points per attempt are 1.124, while actual conversion is −0.60 points per 100 attempts relative to that reference. These are field-goal measures; they exclude turnover and free-throw value.

**Proposed next step:** review calibration and residuals separately by team, zone and recorded action type on a future locked holdout. Examine whether an apparent conversion deficit is concentrated in a recurring shot family. Validate source definitions before comparing seasons. If staffing a full possession-quality model, add the missing scoring and possession-ending channels rather than relabeling this field-goal model.

**What would change the recommendation:** a later-season reversal versus the simple baseline, subgroup miscalibration, source-definition drift or clear evidence that omitted openness/defender-distance information dominates the comparison. Better log loss does not by itself establish a useful basketball decision threshold.

**Interview defense:** the calibration curve groups shots by predicted probability. Its 20 quantile bins are not 20 independent tests, and a visually close aggregate line can conceal subgroup errors. The October visual rebuild recalculated log loss and Brier scores from saved evaluation rows and checked them against the published summary; it did not retrain the large source model.

Sources: [full study](https://github.com/jmsmarrelli/nba-analytics-portfolio/blob/main/reports/05_shot_quality.md), [project source](https://github.com/jmsmarrelli/nba-analytics-portfolio/blob/main/projects/05_shot_quality/analysis.py), [summary](https://github.com/jmsmarrelli/nba-analytics-portfolio/blob/main/projects/05_shot_quality/summary.csv), and [execution limits](https://github.com/jmsmarrelli/nba-analytics-portfolio/blob/main/VALIDATION_CURRENT.md).


---


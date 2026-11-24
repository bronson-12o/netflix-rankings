> **This project is now part of [Analytics Showcase](https://github.com/bronson-12o/analytics-showcase/tree/main/tableau/netflix-rankings).**
> The case study, screenshots, attribution and original history are preserved there. This repository is retained as a read-only historical copy.

# Netflix Top 10 ranking analysis

Tableau coursework exploring which titles rise in the rankings and which stay there.

I compared daily ranking points with observed days in the Top 10. The distinction matters: a ranking is not a count of viewers or hours watched.

![Ranking overview](media/ranking-overview.webp)

## Measures and findings

Each daily appearance receives `11 - [Rank]` points: ten for first place and one for tenth. The supplied observations run April 1, 2020–March 11, 2022. March 2022 is a partial month, and three ambiguous labels are excluded from title comparisons.

Cocomelon appears on 428 observed days and earns 1,474 points. Squid Game earns 495 points across 66 days; Lucifer earns 405 across 56. Points describe ranking strength; observed days describe persistence.

## What I built

Excel ranking records → Tableau daily-point and date calculations → title/month comparisons → ranking overview and persistence dashboard.

I prepared the calculations, compared the two measures, checked the totals, and redesigned the views for a clearer presentation. [Selected calculation](selected-calculations.txt).

## Open and review

Read the overview above and [title-persistence view](media/title-persistence.webp). These are saved exports; the GitHub images do not provide Tableau interaction. See the [portfolio](https://bronsonhatch.com) for the wider case study.

The Tableau workbook and supplied source spreadsheet are maintained privately. This showcase has no installation step and contains no instructor instructions or bulk source dataset.

## Verification and limits

Saved September 2026 evidence records the Excel/extract comparison and independent SQL totals. The September 29 layout review records two dashboards opened in Tableau, unchanged formulas/filters, and sort/undo behavior. The records support the displayed historical analysis; they are not a new Tableau execution during packaging.

The dataset cannot establish audience size, subscriptions, hours watched, or commercial impact. An observed-day count does not imply consecutive days.

[Use and attribution](USE-AND-ATTRIBUTION.md). INFO 4120 coursework; independent student analysis, not a Netflix engagement.

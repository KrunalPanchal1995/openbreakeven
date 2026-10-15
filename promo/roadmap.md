# Roadmap: the path to the openbreakeven Target

This is the path, not the code. Each milestone says what you learn, what you build, and how you know it works. Pick one and open a pull request. See [CONTRIBUTING.md](../CONTRIBUTING.md).

## Session 4: Price and demand move together

**You will learn:** Correlation between random inputs, and how it changes the spread of profit.

**You will build:** A second simulation in which price and demand are negatively correlated (a higher price goes with lower demand).

**Checkpoint (not met by the shipped code):** With correlation -0.5 between price and demand, the loss probability differs from the independent value by at least 2 percentage points (the shipped independent model gives 9.5 percent).

**Difficulty:** intermediate

## Session 5: Shares of the variance

**You will learn:** Variance-based sensitivity: how much of the spread of profit each input explains, not only a one-at-a-time swing.

**You will build:** A function that reports, for price, variable cost and demand, the share of profit variance it explains.

**Checkpoint (not met by the shipped code):** The shares add up to 1 within 0.05 (the shipped tornado gives swings in dollars, not shares).

**Difficulty:** advanced

## Session 6: Seasons and a loan

**You will learn:** Monthly cash flows that are not constant, and borrowing part of the start-up cost (see openloan).

**You will build:** A 12 month demand pattern with a December peak and a loan repaid in equal monthly instalments.

**Checkpoint (not met by the shipped code):** The twelve monthly profits add up to within 1 percent of twelve times the flat monthly profit when the pattern averages 1.0, and the model reports a month-by-month running total (the shipped model uses constant cash).

**Difficulty:** intermediate

## Session 7: Design under a risk limit

**You will learn:** Optimising price and capacity when a probability limit is a hard constraint.

**You will build:** A search that adds new oven options and prices, and reports the cheapest design that meets the limit.

**Checkpoint (not met by the shipped code):** A design with loss probability at most 2 percent and payback at most 10 months, which none of the shipped oven sizes and prices on a 0.05 dollar grid can reach.

**Difficulty:** advanced

## Session 8: A browser lab with live Monte Carlo

**You will learn:** Fast simulation in the browser, and how to make a histogram and a tornado chart redraw on every slider move.

**You will build:** One page with sliders for price, costs, fixed cost and demand, linked to the lines, histogram and tornado chart.

**Checkpoint (not met by the shipped code):** The histogram of 20000 draws redraws in under 100 milliseconds after a slider move, and its loss probability agrees with the Python lesson within 1 percentage point.

**Difficulty:** advanced

## The final step

Combine the milestones: a browser page where sliders move the break-even point while a profit histogram and a tornado chart update, with correlated inputs and a loan. If your result looks like the Target animation, open a pull request and tell us how you did it.

# How fucked am I

A single-page calculator that estimates how much of a tax technology professional's working week an AI could already do, and how that might change over the next few years.

Live site: https://davej91.github.io/howFuckedAmI/

## What it does

You pick a grade, from associate to partner, and adjust how your week splits across seven kinds of work: client advice, technical research, managing projects, creating deliverables, advising on implementation, compliance and calculations, and building tools. Each kind of work is scored by the public AI benchmarks closest to it, such as Vals Tax Agent Bench, TaxCalcBench and the Remote Labor Index. The page weights those scores by your week to give an index out of 100.

You can also project the index forward under a few scenarios for the pace of AI progress, switch individual benchmarks on or off, and choose whether work that no benchmark measures counts as safe or as exposed.

The role mixes are estimates, not timesheet data, and the projections are what-ifs rather than forecasts. It is a side project for curiosity, not advice.

## Running it

There is no build step and no dependencies. Everything (HTML, CSS, JavaScript and the benchmark data) lives in `index.html`.

To run it locally, open `index.html` in a browser, or serve the folder:

```
python3 -m http.server 8000
```

then visit http://localhost:8000.

## Deploying

The site is served by GitHub Pages from the root of the `main` branch. To set it up on a fork, go to Settings, then Pages, choose "Deploy from a branch", and pick `main` and `/ (root)`.

## Updating the figures

The benchmark scores, leaders, dates and sources sit in the data block at the top of the script in `index.html`, between the "Data: update by hand" and "End data" comments. Update them there when the leaderboards move, and change the "Benchmarks checked" date in the page header to match.

## Screenshot

Screenshot to come.

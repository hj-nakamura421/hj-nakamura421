<h1 align="center">HJ Nakamura</h1>

<!-- Public engineering portfolio profile -->

<p align="center">
  <strong>Mechanical Engineering at Imperial College London</strong><br>
  Formula Student EV · vehicle development · engineering analysis and decision tools.
</p>

<p align="center">
  <a href="https://github.com/hj-nakamura421/imperial-fs-telemetry"><strong>Formula Student telemetry</strong></a>
  ·
  <a href="https://uk-renewable-intelligence.github.io/">Live energy platform</a>
  ·
  <a href="https://github.com/hj-nakamura421/uk-renewable-energy-dashboard">Forecasting pipeline</a>
</p>

## What I build

I am interested in vehicle performance, mechanical design, simulation, systems, test and development. I use code as an engineering tool: to turn imperfect data into decisions, expose assumptions, automate repetitive analysis and communicate results clearly.

## Featured vehicle project: Formula Student EV telemetry debrief

[Formula Student EV Drivetrain Telemetry Debrief](https://github.com/hj-nakamura421/imperial-fs-telemetry) is a portfolio prototype for reviewing EV test data.

What I engineered:

- validate signal schemas, numeric quality, timestamps and lap numbering before analysis;
- group consecutive motor-temperature, inverter-temperature and pack-voltage breaches into reviewable events;
- integrate timestamped mechanical and electrical power instead of assuming a fixed logger rate;
- compare lap-level power, temperatures, pack voltage, energy and estimated drivetrain efficiency;
- expose engineering limits and nominal pack voltage as adjustable inputs;
- separate the calculation layer from the interface and verify it with `pytest` and GitHub Actions.

The committed session is explicitly synthetic. It demonstrates the workflow without claiming access to or deployment on private team data.


## Featured system: UK Renewable Infrastructure Intelligence

[UK Renewable Infrastructure Intelligence](https://uk-renewable-intelligence.github.io/) is a deployed screening and forecasting platform for the UK renewable-energy pipeline.

| Current release | Evidence |
|---|---:|
| Public planning records | **13,009** |
| Historical REPD snapshots | **15** |
| Projects with linked forecasts | **6,189** |
| Projects with usable map coordinates | **12,980** |

What I engineered:

- cleaned and reconciled changing Renewable Energy Planning Database extracts;
- reconstructed project histories and stage transitions through time;
- built discrete-time survival forecasts with censoring and temporal holdouts;
- compared empirical, logistic and CatBoost candidates, retaining the simpler baseline when the challenger did not improve Brier reliability;
- separated macroeconomic and policy stress assumptions from the trained forecast;
- shipped a JavaScript and Leaflet public dashboard alongside a Python and Streamlit modelling workbench;
- documented data quality, calibration, model governance and known limitations.

**Explore:** [live platform](https://uk-renewable-intelligence.github.io/) · [methodology](https://github.com/hj-nakamura421/uk-renewable-energy-dashboard/blob/main/METHODOLOGY.md) · [model card](https://github.com/hj-nakamura421/uk-renewable-energy-dashboard/blob/main/MODEL_CARD.md) · [architecture](https://github.com/hj-nakamura421/uk-renewable-energy-dashboard/blob/main/ARCHITECTURE.md)

## Selected engineering projects

| Project | What it demonstrates | Stack |
|---|---|---|
| [Formula Student telemetry](https://github.com/hj-nakamura421/imperial-fs-telemetry) | Drivetrain test analysis, thermal and accumulator event triage, timestamp-aware energy integration and lap summaries | Python, pandas, NumPy, Plotly, Streamlit, pytest |
| [Renewable Intelligence platform](https://github.com/uk-renewable-intelligence/uk-renewable-intelligence.github.io) | Product design, interactive mapping, project screening and decision-focused visualisation | JavaScript, Leaflet, GitHub Pages |
| [Forecasting and data pipeline](https://github.com/hj-nakamura421/uk-renewable-energy-dashboard) | Entity resolution, survival modelling, temporal validation, scenario analysis and reproducibility | Python, pandas, scikit-learn, CatBoost, Streamlit |

## Engineering principles

- **Validate in time.** Random splits are not enough for deployment-style forecasting.
- **Promote on evidence.** A more complex model is useful only when it improves out-of-sample reliability.
- **Expose uncertainty.** Assumptions, missing data and model limitations belong in the interface.
- **Build for inspection.** Clear documentation, tests and reproducible pipelines are part of the product.

## Tools I use

`Python` · `pandas` · `NumPy` · `scikit-learn` · `CatBoost` · `Streamlit` · `Plotly` · `JavaScript` · `Leaflet` · `Git` · `GitHub Actions`

## Placement interests

I am seeking year-placement opportunities across vehicle performance, mechanical design, simulation, systems, test and development, manufacturing and process improvement. For me, computational work is strongest when it supports a physical engineering decision and can be inspected by another engineer.

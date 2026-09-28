<h1 align="center">HJ Nakamura</h1>

<!-- Public engineering portfolio profile -->

<p align="center">
  <strong>Mechanical Engineering at Imperial College London</strong><br>
  Formula Student EV · vehicle development · engineering analysis and decision tools.
</p>

<p align="center">
  <a href="https://imperial-fs-telemetry.streamlit.app/"><strong>Formula Student debrief · synthetic demo</strong></a>
  ·
  <a href="https://uk-renewable-intelligence.github.io/">Live energy platform</a>
  ·
  <a href="https://github.com/hj-nakamura421/uk-renewable-energy-dashboard">Forecasting pipeline</a>
</p>

## What I build

I am interested in vehicle performance, mechanical design, simulation, systems, test and development. I use code as an engineering tool: to turn imperfect data into decisions, expose assumptions, automate repetitive analysis and communicate results clearly.

## Featured vehicle project: Formula Student EV Test-Data Debrief

[Formula Student EV Test-Data Debrief](https://imperial-fs-telemetry.streamlit.app/) is my independent engineering portfolio prototype for turning EV drivetrain telemetry into a structured post-run review. The public demonstration uses synthetic data; **it is not an official Imperial Formula Student tool or team dataset, and has not been deployed by the team.**

**Physical engineering → test data → calculations → engineering judgement → next action.** Each review window connects a signal breach to a specific next investigation, such as checking cooling performance, current demand or pack state of charge.

What I engineered:

- telemetry validation for signal schemas, numeric quality, timestamps and lap numbering;
- event detection that groups motor-temperature, inverter-temperature and pack-voltage breaches into review windows;
- timestamp-aware mechanical and electrical energy integration, with lap-level comparisons;
- a deterministic synthetic generator linking torque, RPM, power, assumed efficiency and a baseline pack-resistance model, with injected review scenarios;
- a Streamlit and Plotly interface with adjustable demonstration thresholds and an exportable review log;
- a separate calculation layer verified with `pytest` and GitHub Actions.

The default temperatures and voltages are illustrative review values, not Imperial Racing Green hardware limits. Priority labels use a documented demonstration heuristic. Real-telemetry validation and hardware-specific thresholds remain future work.

**Review the work:** [screenshot and engineering case study](https://github.com/hj-nakamura421/imperial-fs-telemetry#readme) · [analysis source](https://github.com/hj-nakamura421/imperial-fs-telemetry/blob/main/telemetry.py) · [tests](https://github.com/hj-nakamura421/imperial-fs-telemetry/blob/main/tests/test_telemetry.py)

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
| [Formula Student EV Test-Data Debrief](https://github.com/hj-nakamura421/imperial-fs-telemetry) | Independent prototype with synthetic data: thermal and voltage event review, timestamp-aware energy integration and lap summaries | Python, pandas, NumPy, Plotly, Streamlit, pytest |
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

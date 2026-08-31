<h1 align="center">HJ Nakamura</h1>

<!-- Public engineering portfolio profile -->

<p align="center">
  <strong>Mechanical Engineering at Imperial College London</strong><br>
  Building transparent software for energy infrastructure, engineering data and decision support.
</p>

<p align="center">
  <a href="https://uk-renewable-intelligence.github.io/"><strong>Live energy platform</strong></a>
  ·
  <a href="https://github.com/hj-nakamura421/uk-renewable-energy-dashboard">Forecasting pipeline</a>
  ·
  <a href="https://github.com/hj-nakamura421/imperial-fs-telemetry">Formula Student telemetry</a>
</p>

## What I build

I am interested in the point where physical systems, imperfect data and engineering decisions meet. My projects turn public infrastructure records and vehicle telemetry into tools that can be inspected, tested and used.


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
| [Renewable Intelligence platform](https://github.com/uk-renewable-intelligence/uk-renewable-intelligence.github.io) | Product design, interactive mapping, project screening and decision-focused visualisation | JavaScript, Leaflet, GitHub Pages |
| [Forecasting and data pipeline](https://github.com/hj-nakamura421/uk-renewable-energy-dashboard) | Entity resolution, survival modelling, temporal validation, scenario analysis and reproducibility | Python, pandas, scikit-learn, CatBoost, Streamlit |
| [Formula Student telemetry](https://github.com/hj-nakamura421/imperial-fs-telemetry) | Drivetrain test analysis, thermal monitoring, voltage-sag detection and lap summaries | Python, Plotly, Streamlit |

## Engineering principles

- **Validate in time.** Random splits are not enough for deployment-style forecasting.
- **Promote on evidence.** A more complex model is useful only when it improves out-of-sample reliability.
- **Expose uncertainty.** Assumptions, missing data and model limitations belong in the interface.
- **Build for inspection.** Clear documentation, tests and reproducible pipelines are part of the product.

## Tools I use

`Python` · `pandas` · `NumPy` · `scikit-learn` · `CatBoost` · `Streamlit` · `Plotly` · `JavaScript` · `Leaflet` · `Git` · `GitHub Actions`

## Currently improving

- shareable project and filter URLs;
- historical project timelines and comparable-project evidence;
- faster, lazy-loaded dashboard data;
- calibration views that make forecast reliability understandable to non-specialists.

I am open to engineering, energy, automotive and data-focused internship conversations.

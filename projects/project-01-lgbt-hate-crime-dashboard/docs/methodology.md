### Methodology
The project followed a structured, end‑to‑end data science workflow designed to ensure analytical integrity, transparency, and responsible communication of sensitive data. The methodology combines reproducible data engineering, exploratory analytics, and contextual interpretation.

## 1. Data Acquisition
Publicly available datasets were sourced from:

+ Home Office — police‑recorded hate crime statistics (YE March 2015–2024)
+ ONS — mid‑year population estimates and sexual orientation survey data
+ Electoral Commission & UK Parliament — national election and referendum results

All datasets were aligned to a Year Ending March calendar to ensure temporal consistency across sources.

## 2. Data Engineering & Modelling
Data preparation and modelling were performed in Power BI, using:

+ Power Query for ingestion, cleaning, and harmonisation
+ DAX for analytical measures, time‑based calculations, and association metrics

A star schema was implemented to support clarity and auditability:

+ Fact table — annual LGBT hate crime counts and derived rates
+ Dimension tables — year mapping, population context, political indicators
+ Analysis table — dedicated structure enabling correct evaluation context for correlation and scatter‑based analysis

Key engineering steps included:
+ Normalising year formats across datasets
+ Creating population‑adjusted rates per 100,000
+ Mapping political parties into five analytically meaningful voting blocs
+ Explicitly excluding YE March 2019 due to missing Home Office data

No imputation or interpolation was applied to preserve data integrity.

## 3. Exploratory Data Analysis (EDA)
The analytical approach was deliberately exploratory rather than predictive, reflecting the small number of annual observations.

Techniques included:
+ Trend analysis of counts and population‑adjusted rates
+ Comparative analysis between sexual orientation and transgender hate crime strands
+ Correlation analysis (Pearson) between political context and hate crime metrics
+ Lagged association analysis comparing political conditions in one year with changes in hate crime the following year

All findings were framed as associational, not causal, due to the aggregated nature of the data and the risk of ecological fallacy.

## 4. Dashboard Design & Visual Communication
The dashboard was structured into four narrative pages:

+ Hate Crime Overview — headline KPIs and long‑term trends
+ Population & Identity Context — demographic and identity estimates
+ Political Climate & Associations — voting bloc trends and contextual overlays
+ Analytical Insights — correlation outputs, lagged scatter plots, and methodology notes

Design principles followed Storytelling with Data best practice:

+ Presenting counts and rates together to avoid misinterpretation
+ Embedding explanatory text to prevent visuals being read in isolation
+ Prioritising accessibility, clarity, and responsible communication

## 5. Ethics, Bias & Limitations
The project adhered to UK data ethics principles:

+ Use of public, aggregated data only
+ No individual‑level inference
+ Transparent communication of uncertainty and limitations
+ Avoidance of causal claims

Key limitations include:
+ Missing data for YE March 2019
+ National‑level aggregation limiting statistical power
+ Self‑reported identity estimates subject to measurement uncertainty
+ Potential influence of reporting behaviour and recording practices

These limitations were explicitly acknowledged in the dashboard and accompanying narrative.

## 6. Interpretation & Decision Support
The final dashboard provides a structured framework for:

+ Understanding long‑term LGBT hate crime trends
+ Interpreting changes in the context of population and political shifts
+ Supporting evidence‑based discussion among policymakers and analysts

The methodology ensures that insights remain transparent, reproducible, and responsibly communicated.

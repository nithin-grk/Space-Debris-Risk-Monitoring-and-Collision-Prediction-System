Phase 1: Data Engineering

Load orbital data from:

CelesTrak active satellites
CelesTrak debris groups
Satellite catalog metadata

Output:

Clean satellite table
Clean debris table
Combined orbital object table
Phase 2: Orbital Feature Engineering

Create features such as:

Altitude
Inclination
Eccentricity
Mean motion
Orbital period
Object type
Orbit category: LEO, MEO, GEO
Debris density around each object
Phase 3: Collision Risk Engine

Calculate:

Future object positions
Distance between satellites and debris
Closest approach distance
Relative velocity
Time to closest approach

Then create a risk score from 0 to 100.

Phase 4: Machine Learning

Use ML models to predict risk category:

Low risk
Medium risk
High risk

Models:

Logistic Regression
Random Forest
XGBoost
Isolation Forest for anomaly detection
DBSCAN/K-Means for orbital clustering
Phase 5: Explainable AI

Use SHAP or feature importance to explain:

Why was this satellite classified as high risk?

Example:

Close approach distance is low
Relative velocity is high
Satellite is in a crowded orbital shell
Multiple debris objects are nearby
Phase 6: LLM Assistant

Add an AI assistant that answers:

“Which satellites are highest risk today?”
“Why is this satellite high risk?”
“Which orbital region is most crowded?”
“Summarize today’s debris risk.”
Phase 7: Dashboard

Build a Streamlit dashboard with:

Risk leaderboard
Orbital congestion charts
Close approach table
Anomaly detection results
AI explanation panel
Interactive chat assistant

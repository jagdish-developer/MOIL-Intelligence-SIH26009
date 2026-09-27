# MOIL Intelligence 

AI/ML and Space Technology based decision-support system for manganese
exploration, production shortfall prediction, equipment intelligence,
and exploration planning for MOIL.

**SIH26009 — Using AI/ML and Space Technology to Identify Manganese Reserves and Overcome Production Shortfalls**

MOIL requires improved identification of manganese mineralization and
better prediction of production shortfalls using geological data,
historical production, equipment performance, and satellite/space
technology inputs. :contentReference[oaicite:0]{index=0}

## Core Modules

### Module 1 — Production Shortfall Prediction

Using AI/ML to predict, attribute, and explain manganese production
shortfalls across MOIL's organizational hierarchy — from the CMD/Board
level to the equipment operator.

The module focuses on:

- Production shortfall prediction
- Expected vs actual production analysis
- Structural and execution gap analysis
- Equipment downtime analysis
- Equipment maintenance-risk prediction
- Weather and operational impact analysis
- Root-cause attribution using SHAP
- Role-based decision support
- Equipment redeployment and scheduling inputs

### Organizational Hierarchy

1. CMD / Board
2. Functional Directors
3. Joint GM / Assistant GM — State Cluster
4. Agent / Mine Manager
5. Assistant Manager / Mining Engineer — Section
6. Shift Supervisor / Foreman
7. Equipment Operator

Cross-cutting inputs include:

- Geology / Survey
- Maintenance / Engineering
- Logistics / Rail-Rake Coordination

### ML Stack

| Purpose | Model / Method |
|---|---|
| Production shortfall prediction | XGBoost |
| Equipment maintenance-risk | Random Forest / XGBoost |
| Factor attribution | SHAP |
| Uncertainty estimation | Quantile Regression |
| Demand trend modelling | Time-series / Lag Features |

---

### Module 2 — Manganese Exploration Intelligence

A multi-source geospatial and machine-learning framework for identifying
areas with higher manganese mineralization prospectivity and
prioritizing them for further investigation.

The module focuses on:

- Geological data integration
- Remote sensing / Sentinel-2 processing
- Spectral alteration analysis
- Structural and terrain analysis
- Geophysical evidence integration
- Borehole and assay integration
- Prospectivity mapping
- Confidence and uncertainty estimation
- Exploration target prioritization
- 3D geological context
- Field verification

### Exploration Workflow

```text
Multi-Source Data
        ↓
Preprocessing & Spatial Alignment
        ↓
Feature Extraction
        ↓
Common Spatial Grid
        ↓
Feature Table
        ↓
RF Baseline + XGBoost
        ↓
Spatial Validation
        ↓
Prospectivity Score
        ↓
Confidence + Uncertainty
        ↓
Target Ranking
        ↓
Exploration Priority
        ↓
3D Geological Context
        ↓
Field Verification

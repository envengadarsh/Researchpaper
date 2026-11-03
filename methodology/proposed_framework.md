# Proposed integrated framework for a campus catchment in Bhopal

## Research contribution (to be tested by the completed review)
A decision-oriented framework connecting GIS-derived catchment representation, SWMM runoff and hydraulic routing, constituent-specific pollutant buildup/washoff, event-based monitoring, independent validation, uncertainty analysis and GI/LID scenario assessment.

## Conceptual workflow

```text
Rainfall + DEM + land cover + drainage survey + soil + monitoring
                              |
                              v
GIS catchment characterisation
(subcatchments, slopes, width, imperviousness, flow paths)
                              |
                              v
EPA-SWMM hydrology and hydraulics
(runoff generation, surface routing, nodes, conduits, outfalls)
                              |
                              v
Water-quality representation
(source inventory -> buildup -> washoff -> pollutant routing)
                              |
                              v
Calibration and independent validation
(flow hydrographs + event loads + EMC + pollutographs)
                              |
                              v
Sensitivity and uncertainty assessment
                              |
                              v
Baseline and GI/LID scenario comparison
                              |
                              v
Decision support with limitations and maintenance needs
```

## Minimum site data checklist

| Data | Required detail | Verification |
|---|---|---|
| Catchment boundary | Official boundary and area | GIS/institutional records and field check |
| Topography | DEM, contours, slopes | Document resolution and validate drainage paths |
| Land cover | Roof, road, parking, vegetation, open soil | Recent imagery and ground truth |
| Drainage network | Inlets, manholes, conduits, dimensions, inverts, outfalls | Field survey and drawings |
| Rainfall | Sub-hourly time series for selected events | On-site gauge or authoritative station |
| Runoff | Discharge or stage with rating curve | Field monitoring |
| Water quality | TSS, nutrients, COD/BOD, metals or locally justified constituents | Event-based sampling and laboratory QA/QC |
| Soil | Texture and infiltration | Field infiltration tests / soil survey |
| Operations | Sweeping, sediment removal, maintenance | Facilities records |

Previously discussed approximate area, example subcatchment dimensions, assumed outfall, and assumed parameters are not verified site facts. Do not use them as measured data.

## Proposed modelling steps

1. Confirm study boundary and receiving-water/outfall locations.
2. Prepare and quality-check GIS layers, DEM, land cover and drainage topology.
3. Delineate subcatchments; record the method and spatial resolution.
4. Build the SWMM network with verified geometry and documented parameter sources.
5. Calibrate hydrology using multiple observed rainfall-runoff events; reserve independent events for validation.
6. Select water-quality constituents based on local source inventory and laboratory capacity.
7. Monitor rainfall, flow and event water quality at compatible time steps.
8. Calibrate and independently validate pollutant loads/concentrations where observations allow.
9. Evaluate baseline peak flow, volume, pollutant loads, EMC and first-flush diagnostics.
10. Simulate feasible GI/LID measures with design-specific parameters.
11. Conduct sensitivity and uncertainty analysis and report limitations.

## Candidate research gaps

- Flow calibration does not establish water-quality predictive skill.
- Buildup/washoff parameters may not transfer across constituents and catchments.
- First-flush classification is sensitive to event definitions and sampling frequency.
- Calibrated parameters may not transfer across climate and land-cover scenarios.
- GIS resolution, subcatchment discretisation and impervious connectivity introduce structural uncertainty.
- GI/LID outcomes depend on design, soil, antecedent wetness, maintenance and local rainfall.

## Candidate performance indicators

Use only where data and study design justify them:
- Runoff volume error / percent bias
- Peak discharge error and timing difference
- NSE or KGE (with graphical checks)
- RMSE / MAE
- Pollutant event-load error
- EMC error
- Pollutograph timing and shape
- Cumulative pollutant mass versus cumulative runoff volume

Report units, temporal aggregation, event definition and data split. Avoid using a single goodness-of-fit metric as proof of model adequacy.

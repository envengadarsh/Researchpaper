# Integrated Urban Stormwater Quantity and Quality Modelling Using EPA-SWMM: A Critical Review of Methods, Evidence, Uncertainty and Sustainable Management

**Manuscript type:** Critical review — working draft v0.1  
**Author:** Adarsh Chourasiya [confirm full author details and affiliation]  
**Study context:** Proposed campus-catchment framework for MANIT Bhopal, India.

> **Research integrity statement:** This is a preliminary working draft based on a candidate bibliography and bibliographic/abstract-level evidence. It is not a completed 40-paper full-text review, not a PRISMA-compliant systematic review, and not ready for journal submission. Full-text retrieval, detailed extraction, metadata verification and critical appraisal remain necessary. No site observations, calibrated model outputs or measured findings are claimed.

## Abstract

Urban stormwater runoff is simultaneously a hydrologic response to rainfall and a transport pathway for pollutants accumulated on urban surfaces. Integrated assessment therefore requires a connection between rainfall–runoff generation, drainage hydraulics, pollutant mobilisation, monitoring and sustainable control measures. The US Environmental Protection Agency Storm Water Management Model (EPA-SWMM) is widely applied to urban drainage and low-impact-development scenarios, but prediction quality depends on catchment representation, rainfall inputs, pollutant process assumptions, calibration data and uncertainty. This critical review examines the methodological links between runoff quantity and quality simulation, focusing on pollutant buildup and washoff, event mean concentration (EMC), first-flush diagnostics, GIS integration, calibration/validation, uncertainty and green infrastructure. Foundational reviews establish SWMM's utility for urban hydrology while identifying challenges in diffuse pollutant representation and GI/LID water-quality assessment. Empirical studies indicate that washoff behaviour can differ between particulate and dissolved constituents, while first-flush assessment depends on event definition and monitoring resolution. The paper proposes a decision-oriented framework that links GIS catchment characterisation, SWMM hydrology and hydraulics, constituent-specific quality representation, multi-event evaluation and GI/LID scenario analysis. The framework is intended to guide future work in a campus catchment in Bhopal, India; its application requires verified drainage and land-cover data, local rainfall, runoff observations and event-based water-quality measurements. The evidence synthesis remains preliminary pending full-text appraisal of the candidate literature corpus.

**Keywords:** urban stormwater; EPA-SWMM; runoff modelling; stormwater quality; buildup; washoff; first flush; EMC; GIS; calibration; uncertainty; low impact development.

## 1. Introduction

Urbanisation modifies the partitioning and routing of rainfall through the replacement or fragmentation of pervious surfaces by roofs, roads, parking areas and other impervious surfaces. These changes can increase runoff volume and peak discharge, shorten catchment response time and alter connectivity between pollutant source areas and receiving waters. During dry periods, particulate matter, organic material, nutrients and metals may accumulate on urban surfaces. Rainfall mobilises some of this material and transports it through overland flow and drainage networks. Stormwater management is consequently a coupled quantity-and-quality problem.

Urban stormwater models vary in their spatial and temporal resolution and in their representation of runoff generation, drainage hydraulics and water quality. Zoppou (2001) reviewed urban stormwater models and their capabilities. EPA-SWMM is widely used for urban drainage analysis and scenario assessment. Niazi et al. (2017) reviewed SWMM applications and identified issues relating to model performance, calibration, validation, diffuse pollutant sources, fate and transport, and GI/LID effectiveness.

Hydrologic and water-quality model performance should not be conflated. A reasonable runoff hydrograph fit does not prove that pollutant concentrations or loads are accurate. Quality predictions also depend on source inventories, buildup functions, washoff parameters, pollutant phase, antecedent dry period and sampling design. Chen and Adams (2006) connect rainfall–runoff transformation with pollutant buildup and washoff. Soonthornnonda et al. (2008) report constituent-specific washoff coefficients. Gaut et al. (2019) report differences in washoff-model performance between particulate and dissolved pollutants in their Singapore catchment dataset.

First-flush behaviour concerns the relationship between the fraction of pollutant mass transported and the fraction of runoff volume discharged during an event. Its identification depends on event boundaries, sampling frequency, constituent selection and the quantitative criterion used. Gao et al. (2023) review first-flush characterisation and control, while Perera et al. (2021) examine catchment-based EMC estimation and its implications for first-flush assessment.

### 1.1 Aim and objectives

The aim is to critically review methods and evidence for integrated urban stormwater quantity and quality modelling using EPA-SWMM and to formulate a transparent framework for a future campus-catchment application in Bhopal.

Objectives are to:
1. Review SWMM hydrologic and hydraulic representation.
2. Examine pollutant buildup, washoff, EMC and first-flush methods.
3. Evaluate calibration, validation, sensitivity and uncertainty practices.
4. Examine GIS-derived catchment characteristics and drainage representation.
5. Synthesise evidence on GI/LID strategies.
6. Identify data and methodological requirements for a campus application.

## 2. Review methodology

The intended design is a critical integrative review. Search sources should include Scopus, Web of Science, Engineering Village, ASCE Library, ScienceDirect, SpringerLink, Wiley, Taylor & Francis and Crossref, with Google Scholar used for supplementary citation chasing. Search strings should combine SWMM/urban stormwater with water quality, pollutant buildup/washoff, calibration/validation, uncertainty, first flush/EMC, GIS and GI/LID. Exact database queries, dates, filters and result counts must be retained.

Eligible sources should primarily be peer-reviewed journal articles and substantive reviews, including foundational studies. Duplicate or unverifiable records and studies without relevant transferable stormwater insight should be excluded. For each included study, extract the full citation and DOI, location, catchment scale, rainfall and monitoring design, model/version, constituents, parameterisation, calibration/validation, metrics, uncertainty methods, GI/LID practices and limitations.

If the final review is conducted systematically, report the process transparently using PRISMA 2020 (Page et al., 2021). PRISMA is a reporting guideline; it does not replace search execution, screening or critical appraisal. The current 40-paper bibliography is a candidate register, not a completed sample of fully reviewed studies.

## 3. Urban stormwater quantity and quality processes

### 3.1 Rainfall–runoff transformation

Rainfall excess is converted to surface runoff through interception, depression storage, infiltration and surface routing. Impervious fraction and effective impervious connectivity influence runoff generation. Slope, characteristic width, roughness and storage affect hydrograph timing and shape. Subcatchment parameters are often effective representations and should not be presented as direct measurements unless supported by spatial data or field survey.

### 3.2 Drainage hydraulics

Urban drainage systems route runoff through junctions, conduits, storage elements and outfalls. Inaccurate invert elevations, conduit dimensions, connectivity or inlet representation can compromise surcharge, flooding and travel-time predictions. Model network topology should be checked against field surveys and drainage drawings.

### 3.3 Pollutant sources and transport

Pollutant sources vary with land use and surface type. Roads and parking areas may contribute suspended solids and particle-associated metals; roofs and landscaped surfaces may contribute different constituents. Pollutant load is the time integral of concentration multiplied by discharge. Concentration alone does not quantify exported mass.

## 4. Pollutant buildup and washoff

Buildup functions represent accumulation of pollutant mass during dry periods. Washoff functions represent mobilisation and removal during rainfall and runoff. Common formulations include power, exponential and saturation-type buildup and exponential or rating-type washoff. Their parameters are effective and require site- and constituent-specific justification.

Chen and Adams (2006) integrate rainfall–runoff transformation with pollutant buildup and washoff in analytical models. Soonthornnonda et al. (2008) estimate washoff coefficients for several pollutant groups and demonstrate constituent differences. Wang et al. (2011) compare models with and without residual pollutant after storms, highlighting the importance of event-to-event pollutant memory. Gaut et al. (2019) evaluate an exponential washoff model for six pollutants using 126 rainfall events from 12 Singapore sites; their reported performance was stronger for particulate than dissolved pollutants.

A credible SWMM quality application should document the constituent, units, source-area assignment, buildup and washoff functions, parameter source, antecedent dry period, residual-mass assumption, time-step compatibility, and calibration/validation evidence. Parameters should be treated as uncertain when monitoring is limited.

## 5. EMC and first flush

EMC is a flow-weighted mean concentration over a defined runoff event:

\[
EMC = \frac{\int_{t_0}^{t_1} C(t)Q(t)\,dt}{\int_{t_0}^{t_1} Q(t)\,dt}
\]

where C(t) is concentration and Q(t) is discharge. EMC supports event-load estimation but can conceal short-lived concentration peaks. First flush is commonly examined using cumulative pollutant mass fraction versus cumulative runoff-volume fraction. Event definition, sample interval and criterion must be stated. Gao et al. (2023) review first-flush quantification; Perera et al. (2021) report that rainfall and catchment characteristics influence EMC and first-flush interpretation.

Event sampling should capture the rising limb and later hydrograph periods. Flow and sample timing should be synchronised. Report rainfall depth, intensity, duration, antecedent dry period, runoff volume and event boundaries. Flow-weighted composites can be supplemented by discrete high-frequency samples where feasible.

## 6. Calibration, validation and uncertainty

Calibration seeks parameter values that improve agreement between simulated and observed variables; validation tests performance on data not used in fitting. A defensible approach uses multiple events and reports flow and quality performance separately. Potential indicators include NSE, KGE, R², RMSE, MAE and percent bias, but graphical hydrograph/pollutograph checks and mass balance should complement summary metrics.

Sytsma et al. (2022) investigate uncertainty from non-transferable SWMM calibrations across climate and land-cover scenarios. This cautions against assuming calibrated effective parameters remain valid under changed forcing or catchment conditions. Uncertainty sources include rainfall variability, monitoring error, water-quality sampling, delineation, parameter equifinality, network data and model structure. Sensitivity analysis should prioritise parameters relevant to the management decision.

## 7. GIS and catchment representation

GIS supports catchment delineation, slope and area estimation, land-cover mapping, imperviousness assessment and drainage-network analysis. DEM resolution, conditioning, coordinate reference system, ground truth and outlet assignment influence delineation. Roofs, roads, parking, landscaped spaces and open ground should be mapped as distinct classes when their hydrologic or pollutant characteristics justify separation. Subcatchment width and impervious connectivity should be documented as derived or calibrated quantities, not assumed observations.

## 8. Green infrastructure and LID

GI/LID measures reduce or delay runoff through infiltration, storage, evapotranspiration and retention. Candidate practices include green roofs, permeable pavements, bioretention, rain gardens, vegetated swales and detention. Performance depends on design, soil properties, storage, underdrains, antecedent moisture, rainfall and maintenance. Ekmekcioğlu et al. (2021) examine LID strategies using auto-calibrated SWMM. Hydrologic benefits should be distinguished from pollutant-removal benefits; a modelled scenario is not field validation.

## 9. Preliminary research gaps

The candidate literature suggests several gaps for testing in the completed review:
- Flow calibration does not establish water-quality predictive skill.
- Buildup/washoff parameters may not transfer across constituents and catchments.
- First-flush classification depends on sampling design and event definitions.
- Calibrated parameters may not transfer across climate and land-cover scenarios.
- GIS resolution and drainage connectivity introduce structural uncertainty.
- GI/LID performance depends on design, soils, antecedent wetness and maintenance.

## 10. Proposed framework for a campus catchment in Bhopal

The proposed sequence is: (1) verify the study boundary, drainage network and receiving points; (2) obtain sub-hourly rainfall; (3) prepare DEM, land-cover and drainage GIS layers; (4) delineate subcatchments and construct the SWMM network; (5) calibrate and independently validate hydrology using observed events; (6) select quality constituents based on source inventory and laboratory capacity; (7) undertake event-based sampling; (8) calibrate and validate pollutant loads and concentrations where data permit; (9) evaluate baseline peak flow, runoff volume, pollutant loads, EMC and first flush; and (10) assess feasible GI/LID scenarios with uncertainty analysis.

No numerical results are reported because verified site datasets and calibrated model outputs have not been supplied. Previously discussed approximate campus area, example subcatchment dimensions and assumed outfall/parameters must be independently verified before use.

## 11. Limitations and conclusion

This draft is limited by an incomplete search and pending full-text extraction. It does not report completed PRISMA counts or formal quality appraisal. The proposed campus framework remains a research plan pending verified boundary, drainage, rainfall, flow and water-quality observations.

Integrated stormwater assessment requires a defensible connection between rainfall, catchment representation, drainage hydraulics, pollutant source areas, buildup/washoff, monitoring and model evaluation. SWMM is a useful platform for urban hydrology and drainage analysis, but water-quality predictions are sensitive to constituent behaviour, data availability and parameter assumptions. First-flush assessment requires time-resolved event information, and calibrated parameters should be treated cautiously under changed rainfall or land cover. GIS and GI/LID scenarios can support planning when data and physical assumptions are transparent.

## References (anchor references; expand after full-text verification)

Chen, J., & Adams, B. J. (2006). Analytical urban storm water quality models based on pollutant buildup and washoff processes. *Journal of Environmental Engineering*, 132(10), 1314–1330. https://doi.org/10.1061/(ASCE)0733-9372(2006)132:10(1314)

Ekmekcioğlu, Ö., Yılmaz, M., Özger, M., & Tosunoğlu, F. (2021). Investigation of the low impact development strategies for highly urbanized area via auto-calibrated SWMM. *Water Science and Technology*, 84(9), 2194–2213. https://doi.org/10.2166/wst.2021.432

Gao, Z., Zhang, Q., Li, J., Wang, Y., Dzakpasu, M., & Wang, X. C. (2023). First flush stormwater pollution in urban catchments: A review of its characterization and quantification towards optimization of control measures. *Journal of Environmental Management*, 340, 117976. https://doi.org/10.1016/j.jenvman.2023.117976

Gaut, J., Chua, L. H. C., Irvine, K. N., & Le, S. (2019). Modelling the washoff of pollutants in various forms from an urban catchment. *Journal of Environmental Management*, 246, 374–383. https://doi.org/10.1016/j.jenvman.2019.05.118

Niazi, M., Nietch, C., Maghrebi, M., Jackson, N., Bennett, B. R., Tryby, M., & Massoudieh, A. (2017). Storm Water Management Model: Performance Review and Gap Analysis. *Journal of Sustainable Water in the Built Environment*, 3(2). https://doi.org/10.1061/JSWBAY.0000817

Page, M. J., et al. (2021). The PRISMA 2020 statement: An updated guideline for reporting systematic reviews. *BMJ*, 372, n71. https://doi.org/10.1136/bmj.n71

Perera, T., McGree, J., Egodawatta, P., Jinadasa, K. B. S. N., & Goonetilleke, A. (2021). Catchment based estimation of pollutant event mean concentration (EMC) and implications for first flush assessment. *Journal of Environmental Management*, 279, 111737. https://doi.org/10.1016/j.jenvman.2020.111737

Soonthornnonda, P., Christensen, E. R., Liu, Y., & Li, J. (2008). A washoff model for stormwater pollutants. *Science of the Total Environment*, 402(2–3), 248–256. https://doi.org/10.1016/j.scitotenv.2008.04.036

Sytsma, A., et al. (2022). Quantifying the uncertainty created by non-transferable model calibrations across climate and land cover scenarios: A case study with SWMM. *Water Resources Research*. https://doi.org/10.1029/2021WR031603

Wang, L., Wei, J., Huang, Y., Wang, G., & Maqsood, I. (2011). Urban nonpoint source pollution buildup and washoff models for simulating storm runoff quality in the Los Angeles County. *Environmental Pollution*, 159(7), 1932–1940. https://doi.org/10.1016/j.envpol.2011.03.019

Zoppou, C. (2001). Review of urban storm water models. *Environmental Modelling & Software*, 16(3), 195–231. https://doi.org/10.1016/S1364-8152(00)00084-0

# Full-text appraisal — integrated stormwater quantity and quality review

**Appraisal date:** 3 November 2026  
**Review scope:** Integrated urban stormwater quantity and quality modelling, with EPA-SWMM as the principal modelling platform.  
**Evidence rule:** Direct findings are distinguished from our interpretation. This file does not imply that all candidate papers have been appraised.

## Appraisal 1 — Niazi et al. (2017)

**Reference:** Niazi, M., Nietch, C., Maghrebi, M., Jackson, N., Bennett, B. R., Tryby, M., & Massoudieh, A. (2017). Storm Water Management Model: Performance Review and Gap Analysis. *Journal of Sustainable Water in the Built Environment*, 3(2). https://doi.org/10.1061/JSWBAY.0000817

**Access status:** Full article text indexed in PubMed Central (author manuscript); publisher record checked. The accessible indexed full text was read.

### Purpose and review design
The paper reviews SWMM development and applications, with particular emphasis on model performance evaluation, calibration and validation in peer-reviewed literature. It also examines SWMM's water-quality capability and GI/LID effectiveness. The authors report identifying more than 150 peer-reviewed application papers for broader review; 93 publications presented formal model-evaluation statistics and were collated for performance analysis. Conference proceedings were excluded from the performance-statistics collation.

### Main evidence relevant to integrated modelling
- Of the 93 papers reporting formal model evaluation, 67 evaluated runoff prediction. Only 26 formally evaluated water-quality endpoints; 22 of those also evaluated runoff. Coupled quantity–quality evaluation was therefore less common than hydrologic evaluation alone in the reviewed corpus.
- TSS and BOD were evaluated most often (22 and 11 studies, respectively); nutrients and metals were evaluated in fewer studies. The evidence base does not support assuming all pollutant classes are equally well represented or validated.
- The review describes two broad approaches to water-quality analysis: (i) post-processing or coupling an external quality model to runoff outputs, and (ii) using SWMM's internal water-quality modules. These approaches must be distinguished in our synthesis.
- SWMM's computational parsimony is a strength for medium- and large-scale hydrologic applications. The same simplification can constrain representation of spatially diffuse pollutant sources, contaminant fate and transport, and GI/LID treatment mechanisms.
- Identified gaps include parameter estimation, sensitivity analysis, automated calibration, uncertainty assessment, surface heterogeneity, reactive multi-component contaminant processes, land-management operations, and interflow/groundwater pathways.

### Critical appraisal
**Strengths:** Broad review of SWMM application history; explicit attention to formal model evaluation; distinguishes hydrologic and water-quality endpoints; identifies structural as well as practical modelling gaps.

**Limitations:** The underlying studies are heterogeneous in catchment scale, constituents, model configuration and evaluation practice. The count of papers evaluating water quality is not proof of strong model performance. This is a 2017 synthesis and must be complemented by later evidence. Its broad conclusions should not be transferred uncritically to tropical monsoon catchments.

**Interpretation for this review:** A defensible integrated SWMM study should evaluate runoff volume, peak flow and timing alongside constituent concentration and event load. Hydrology-only calibration is insufficient when water-quality predictions are a primary outcome. Record whether each study uses native SWMM buildup/washoff, external post-processing, or model coupling.

**Extraction status:** Full-text appraised. Detailed numerical performance statistics from individual application studies cited within Niazi et al. have not yet been independently extracted.

## Appraisal 2 — Razguliaev et al. (2024)

**Reference:** Razguliaev, N., Flanagan, K., Muthanna, T., & Viklander, M. (2024). Urban stormwater quality: A review of methods for continuous field monitoring. *Water Research*, 249, 120929. https://doi.org/10.1016/j.watres.2023.120929

**Access status:** Full open-access publisher-version PDF retrieved from the Luleå University of Technology DiVA repository and read.

### Purpose and review design
This critical review evaluates continuous, high-temporal-resolution, in-situ stormwater quality monitoring. The authors searched Web of Science and Scopus up to spring 2023, manually screened articles, and added studies through reference-list and citation searching. The final selection contained 84 articles representing 56 independent studies; some papers shared sites and datasets. Studies covered 16 countries, while tropical climates and low- and middle-income countries were under-represented.

### Main evidence relevant to integrated modelling
- Stormwater quality varies between sites, between events and within individual events. Higher temporal resolution is needed to characterise pollutant dynamics and develop and validate reliable stormwater-quality models.
- The review reports eight water-quality parameters directly measured on-site for extended periods. Turbidity and electrical conductivity were most common; other measured variables included pH, dissolved oxygen, light absorbance, fluorescent dissolved organic matter and selected inorganic nitrogen species. Many pollutants are inferred indirectly from proxy measurements.
- Indirect measurements require site-specific relationships between sensor signals and target pollutants. A global calibration may under- or over-estimate values under local stormwater conditions.
- Field problems include variable/intermittent flow, debris and sediment, harsh environmental conditions, equipment and power failures, data transmission and human/maintenance factors.
- The authors emphasise regular calibration, cleaning, inspection, data validation and explicit acknowledgement of uncertainty. Documentation of these practices was inconsistent; only a few studies achieved high scores on their combined best-practice assessment.
- Water-quality monitoring must be accompanied by water-quantity measurements. Flow data are necessary for converting concentration observations into pollutant loads and interpreting quality dynamics.

### Critical appraisal
**Strengths:** Multi-database search description; substantial evidence map; separates direct from indirect measurements; discusses field deployment, maintenance, calibration, validation and uncertainty.

**Limitations:** The review focuses on monitoring technology, not SWMM model structure or hydrologic calibration. It is not a direct comparison of pollutant models. Tropical climates and low-/middle-income settings are under-represented, limiting direct transfer to Indian monsoon catchments.

**Interpretation for this review:** Monitoring design is a core part of integrated model design. A practical SWMM calibration dataset should synchronise rainfall, water level/discharge and event-based water-quality samples; proxy sensor data need local laboratory calibration and quality-control records. Event loads should be calculated from paired concentration and flow observations, with uncertainty propagated or explicitly discussed.

**Extraction status:** Full-text appraised. Site-specific sensor performance values and all individual-study details have not been separately extracted.


## Appraisal 3 — Bhusal and Muthukumaran (2026)

**Reference:** Bhusal, M. R., & Muthukumaran, S. (2026). Event Mean Concentration-based Modelling Approach for a Large Scale Spatially Heterogenous Catchment using SWMM. *Water Resources Management*, 40, Article 55. https://doi.org/10.1007/s11269-025-04407-z

**Access status:** Full open-access article read from the publisher page.

### Purpose and study design
The study evaluates SWMM 5.2 for continuous rainfall–runoff modelling and uses an event mean concentration (EMC) approach to estimate total nitrogen (TN) and total phosphorus (TP) wash-off in the Maribyrnong catchment, Australia. The catchment area is approximately 1,450 km². The authors delineated nine subcatchments using GIS and represented ten land-use classes. Rainfall, land-use, soil/infiltration and stream-network information were assembled from regional datasets. The data were split into a six-month warm-up period, two years for calibration and the remaining period for validation.

The model's hydrology was calibrated and validated at the downstream Maribyrnong River location. Water-quality validation was conducted for TN concentration only; TP could not be validated because observed TP data were unavailable. The authors used literature-derived EMC values and sensitivity scenarios with increased TN EMC.

### Main reported results
- Hydrologic calibration: R² = 0.551, NSE = 0.522, KGE = 0.724 and PBIAS = 3.96%.
- Hydrologic validation: R² = 0.6695, NSE = 0.603, KGE = 0.503 and PBIAS = 19.03%. The paper also reports poor logNSE performance, partly associated with very low flow values.
- TN water-quality validation used 22 observed concentration values. R² remained 0.41 across the three EMC scenarios, while PBIAS improved from -56.47% to -39.24% and -21.7% as the assumed EMC was increased.
- TN wash-off was strongly correlated with impervious runoff volume (r = 0.96). The study also found that simple pervious/impervious grouping was insufficient to explain all nutrient wash-off patterns; more detailed land-use disaggregation was informative.
- The authors conclude that EMC-based modelling can be useful where buildup/washoff data are scarce, but static EMC values can fail to reproduce temporal concentration dynamics. They recommend further development of dynamic EMC values.

### Critical appraisal
**Strengths:** Uses a recent SWMM version; combines GIS-derived catchment heterogeneity, continuous hydrologic simulation and pollutant wash-off; reports separate hydrology and water-quality evaluation; makes the limits of data availability visible rather than claiming full validation.

**Limitations and interpretation risks:**
1. Water-quality validation is limited to 22 TN concentration observations; TP is not validated. Therefore the paper is not evidence of equally robust validation for both nutrients.
2. Calibration occurs at the downstream river location. The authors acknowledge that this localized calibration can leave uncertainty in upstream subcatchment flow and pollutant contributions.
3. The paper reports rainfall inputs described as hourly, but also describes the values as cumulative 24-hour rainfall normalized at 9 a.m. This temporal-resolution description should be checked carefully before using the rainfall setup as a precedent for event-scale modelling.
4. The catchment is very large and contains both urban and non-urban areas. Its scale and routing representation differ substantially from a campus catchment with a defined engineered drainage network.
5. Literature-derived EMCs reduce local monitoring requirements but introduce transferability uncertainty. Improving PBIAS by changing assumed EMC values does not, by itself, demonstrate that event timing or concentration dynamics are reproduced; R² remained unchanged in the scenarios.

**Interpretation for this review:** This paper is a useful recent case study for the trade-off between process-based buildup/washoff parameterisation and the simpler EMC approach. It supports the need to (i) disaggregate meaningful land-use classes, (ii) retain runoff volume in pollutant-load interpretation, (iii) validate each pollutant separately, and (iv) distinguish long-term average load estimation from event-specific pollutograph prediction. For a smaller Bhopal campus application, the paper's large-scale catchment structure should not be copied directly.

**Extraction status:** Full-text appraised. Supplementary tables and raw data were not independently downloaded; reported metrics and design details above are from the article text.


## Cross-paper synthesis: implications for the review

1. **Coupled evaluation is less common than runoff evaluation alone.** Niazi et al. report 26 water-quality evaluations compared with 67 runoff evaluations, with 22 evaluating both. The manuscript should assess the balance between hydrologic and quality validation.
2. **Monitoring constrains model credibility.** Razguliaev et al. show why high-frequency, quality-controlled observations matter: pollutant concentrations change within events, proxy relationships are site-specific, and sensor uncertainty can be substantial.
3. **Concentration is not load.** A quantity–quality synthesis must distinguish concentration prediction from mass-load prediction. Load requires flow and concentration to be integrated over time.
4. **Particulate and dissolved constituents require separate scrutiny.** Candidate washoff studies suggest that a single solids-based relationship may not describe dissolved nutrients or other dissolved pollutants. This remains abstract-level evidence until those individual papers are full-text appraised.
5. **Monsoon transferability is a research gap to test, not an assumed result.** The monitoring review identifies under-representation of tropical climates and low-/middle-income countries. Indian studies should be compared on rainfall regime, antecedent dry period, land use, drainage connectivity, constituent suite and sampling frequency.

## Working appraisal rubric for subsequent papers

Each paper will be appraised against the following dimensions, using **0 = not reported/weak, 1 = partly reported, 2 = clearly reported and appropriate**. Scores are descriptive prompts, not a validated universal quality scale.

| Dimension | Appraisal question |
|---|---|
| Study design and context | Is the catchment, land use, scale and study period described sufficiently? |
| Rainfall and runoff data | Are rainfall resolution, flow measurement and event selection documented? |
| Water-quality data | Are constituents, sampling frequency, laboratory methods and QA/QC described? |
| Model structure | Are hydrology, hydraulics and water-quality processes identified clearly? |
| Parameterisation | Are parameter sources, assumptions and physical plausibility explained? |
| Calibration | Are calibration data, objective functions and endpoints appropriate? |
| Validation | Is validation independent in time or event, and are both quantity and quality assessed? |
| Uncertainty and sensitivity | Are input, parameter, structural and measurement uncertainties considered? |
| Transferability | Are climate, catchment and operational limits discussed? |
| Reproducibility | Are model version, input data, configuration and sufficient details available? |

Do not collapse these dimensions into a single score without explaining weighting. A paper with strong hydrology calibration but no quality validation must not be described as a fully validated integrated quantity–quality model.

<figure>
  <img src="logo-climate-data-ca-1-smaller.png" alt="logo" style="width:10%">
</figure>

# Canadian Centre for Climate Services Data Standards
# Version 0.0.2

## Summary and Objectives
Climate data is increasingly used by users across Canada for consequential decisions around climate change risk, adaptation and resilience.  The [Canadian Centre for Climate Services (CCCS)](https://www.canada.ca/en/environment-climate-change/services/climate-change/canadian-centre-climate-services.html) is a key developer and distributor of this information, and it aims to develop and maintain accessible, transparent, trustworthy, and well-documented datasets.  To support this goal, this document defines a specific set of standards for all new quantitative data being developed for inclusion on ClimateData.ca and/or the CCCS website.  Barring exceptional circumstances, these standards must be met or exceeded for all data being considered for [ClimateData.ca](https://climatedata.ca/) or the [CCCS website](https://www.canada.ca/en/environment-climate-change/services/climate-change/canadian-centre-climate-services.html), whether the data is developed by CCCS, federal, regional or provincial partners, academia, the private sector, or multi-stakeholder groups.  Proactive communication and regular mid-project data standards checks will ensure high quality data products and reduce the risk of potential late-stage data rejection.  Meeting or exceeding these standards will ensure that all new products distributed by the CCCS support the objective “to provide Canadians with information and support to consider climate change in their decisions”.

Where possible, the standards presented here align with broader national and international data standards initiatives.  This standards document itself is versioned according to [Semantic Versioning (semver)](semver.org) and shared in a version controlled manner using [Git](github.com).  Suggestions for new standards or modifications to the current standards are welcome and may be submitted via [Git pull requests](https://docs.github.com/en/free-pro-team@latest/github/collaborating-with-issues-and-pull-requests/about-pull-requests).

## Data Standards

### Documentation
The data must be associated with documentation that provides:
1. A clear, up-to-date, plain language executive summary that describes what the data tangibly represents; (*Mandatory*)
2. A complete and up-to-date general and technical description that addresses the topic of each section of this data standards document; (*Mandatory*)
3. At least one previous formal publication or report describing the methodology/data, or use of the methodology/data in a scientific or applied setting. (*Mandatory*)
4. At least one plain language guidance document outlining key background, considerations and processes (see Relation to User Needs - item 3) relevant to this data. (*Mandatory*)  

### Relation to User Needs
The data must be associated with documentation that describes:
1. How the data itself, and/or specific delivery of the data on ClimateData.ca or the CCCS website, addresses (in whole or in large part) a documented need of one or more Canadian user groups; (*Mandatory*)
2. Why providing the data on ClimateData.ca or the CCCS website provides benefits relative to other existing datasets, or via delivery of the same data by other methods; (*Recommended*)
3. How the data: (*Mandatory*)
   1.	Can be demonstrably applied to support user needs, or;
   2.	Requires further processing (e.g. via additional quantitative analysis or as use as input into an impacts model ).  If further processing is required, a description of the full processing workflow must be provided, along with a demonstration that this workflow is (or could in the near future) be feasible to undertake by all identified user groups.    
   3. should not be applied (e.g. potential user needs for which the data was not intended) 
4. A specific case study/example that demonstrates how users have already used, or would use, the data. (*Recommended*)

### Scientific Integrity
The data must be associated with documentation (or references to previous documentation) that:
1. Provides scientific justification of methods used to develop the data.  It must include at a minimum: (*Mandatory*)
   1. A qualitative review of the methods compared to other contemporary/similar methods and approaches
   2. An assessment of the methods against fundamental scientific theory and understanding;
   3. An objective critique of methods strengths and weaknesses; 
2. Provides quantitative assessment of the resulting data.  This must include:  (*Mandatory*)
   1. For data based on historical observations:
      1. Wherever possible and feasible, comparisons to independent observations or models to indicate measures of bias, particularly relative to the maximum bias that would be acceptable to users;
      2. Quantification of key data statistics, including (but not limited to) measures of averages, ranges, outliers, trends, and missing data;
   2. For future projections:  
      1. Wherever possible, assessment of future values for realistic trends, ranges, and statistics;
      2. Comparison to any similar (‘apples-to-apples’) datasets;
3. Describes an agreement for data developers to provide as-needed support and/or training for CCCS Support Desk staff in responding to data/methods queries;(*Recommended*)
4. Identifies one or more reviewers who could review, or already have reviewed, the data for scientific integrity. (*Recommended*)

### Availability and Licensing
The data must be:
1. Free of cost; (*Mandatory*)
2. Available for unrestricted use that meets [ClimateData/CCCS data distribution policies and licenses](https://climatedata.ca/legal/).  Data must be available for commercial use where commercial fees relate specifically to added value (e.g. reformatting/reorganizing/aggregation, advanced interpretation, integration into risk assessments, etc.) and not to data resale.  Licensing that meets this data standard requirement includes (but is not limited to) the [Creative Commons Attribution 4.0 International Public License](https://creativecommons.org/licenses/by/4.0/legalcode), and for data produced by ECCC, the [License Agreement for Use of Environment and Climate Change Canada Data](https://climate.weather.gc.ca/prods_servs/attachment1_e.html) and the [Open Government License - Canada](https://open.canada.ca/en/open-government-licence-canada). (*Mandatory*)
3. Findable

### Provenance and Reproducibility
The data must be:
1. Versioned using a consistent tracking protocol (e.g. [Semantic Versioning (semver)](semver.org) that identifies major/minor data revisions, for data versions hosted both at CCCS and elsewhere.  Enumerated data versions should be associated with the following [World Meteorological Organization WMO-suggested items](https://library.wmo.int/doc_num.php?explnum_id=7867): (*Mandatory*)
   1. The time at which the data was produced;
   2. Who (at the individual and organizational level) produced and is responsible for the data;
   3. What sources (e.g. models, observational instruments, etc.) the data was derived from;
   4. How/why the data changed relative to previous data versions (if applicable);
2. Reproducible through application of original underlying tools, including code, scripts, and/or documented workflows.  All tools must be made available to the portal partners upon request and be complete, version controlled and self-documented to the extent that a knowledgeable 3rd party (for example, an expert witness in a court proceeding) would not require additional information to reproduce a particular version of the data. (*Recommended*)

### Data Coverage and Resolution 
The data must:
1. Cover the entire Canadian landmass or significant regions thereof, and/or coastal and offshore regions if required for maritime-specific user needs; (*Mandatory*)
2. For gridded information: be at a spatial resolution that is directly applicable to identified user needs and, if feasible, be at the same resolution as existing ClimateData.ca products; (*Mandatory*)
4. Cover at a minimum: (*Mandatory*)
   1. For climate models: the years 1950-2100 at a minimum;
   2. For observationally-sourced data: should cover at least 30 years and cover a period that is applicable to identified user needs;
5. Represent information at a temporal resolution that is directly applicable to identified user needs. (*Mandatory*)

### Uncertainty Quantification
The data itself, or supporting datasets or documentation, must allow CCCS staff and users to understand sources of uncertainty.  'Uncertainty' can take different forms depending on the data in question.  Depending on the data set, sources of uncertainty that should be adressed could include:
1. Observations: for data derived from observations or data that indirectly incorporates observations (e.g. reanalysis data), the effect of uncertainties (e.g. observational bias and error, uncertainty in data processing methods) should be qualitatively explained and if possible quantified; (*Mandatory*)
2. Future projections: for data derived from climate model simulations, three sources of uncertainty should be addressed: (*Mandatory*)
   1. Model uncertainty, via either: 
      1. a large ensemble of models in agreement with current multi-model project frameworks;
      1. an [objective model selection process](https://doi.org/10.1175/JCLI-D-14-00636.1);
   2. Scenario uncertainty: for data derived from climate model simulations, scenario-distinct data should be provided that is consistent with as many of the following scenarios as possible:
      1. RCP2.6, RCP4.5, and RCP8.5 scenarios, or;
      1. SSP1-2.6, SSP2-4.5, SSP3-7.0, and SSP5-8.5 scenarios;
   3. Internal variability uncertainty, via ensemble simulations or other equivalent approaches.

### Metadata  
Data metadata (information describing the data) must: 
1. Conform to [Climate and Forecasting (CF) Conventions](https://cfconventions.org/) or other case-specific metadata standards that provide clear information on what the dataset represents.  Where data is meteorological or climatological and provided in netCDF format (preferred), CF Convention compliance is recommended as a minimum standard.  For other data formats, general CF Convention metadata guidelines should be followed to all extents possible (for example, variable and data dimension names should use standard naming formats, even if these are captured via standardized file naming conventions);(*Mandatory*)
2. To all extents possible, leverage metadata capabilities of files formats to integrate metadata in the data files themselves;(*Recommended*)
3. Be associated with an accurate description of number of files and total dataset size (e.g. megabytes, gigabytes); (*Mandatory*)
4. Include information pertaining to: (*Mandatory*)
   1. licensing;
   2. provenance

### File Format
1. Be in one of the following file formats: (*Recommended*)
   1. netCDF;
   2. text (CSV);
   3. GeoJSON;
   4. GeoTIFF;
   5. Shapefile;

### Quality Assurance/Quality Control Review
The data must be associated with certifying documentation:
1. Confirming that a quality assurance review has assessed that no errors are known to exist in the data creation methodology; (*Mandatory*)
2. Confirming that a quality control review has assessed that no errors are known to exist in the final data and metadata. (*Mandatory*) 

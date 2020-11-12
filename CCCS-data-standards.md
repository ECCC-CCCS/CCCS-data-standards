# Canadian Centre for Climate Services Data Standards (*Version 0.0.1*)
## Summary and Objectives
Climate data is increasingly used to by users across Canada for consequential decisions around climate change risk, adaptation and resilience.  The [Canadian Centre for Climate Services (CCCS)](https://www.canada.ca/en/environment-climate-change/services/climate-change/canadian-centre-climate-services.html) is a key developer and distributor of this data, and is therefore responsible for developing and maintaining accessible, transparent, trustworthy, and well-documented datasets.  To support this responsibility, this document defines a specific set of agreed-upon standards for all new quantitative data being developed for inclusion on ClimateData.ca and the CCCS website.  Barring exceptional circumstances, these standards must be met or exceeded for all data being considered for [ClimateData.ca](https://climatedata.ca/) or the [CCCS website](https://www.canada.ca/en/environment-climate-change/services/climate-change/canadian-centre-climate-services.html), whether the data is developed by CCCS, federal, regional or provincial partners, academia, the private sector, or multi-stakeholder groups.  It is possible that different standards for a particular dataset could be addressed by a range of groups: for example, CCCS outreach/engagement staff may address user needs standards, academic partners may address scientific integrity standards, and CCCS technical partners may address metadata, provenance and reproducibility standards.  Ultimately, it is not so important who addresses each standard, so much as it is that each standard is ultimately met or exceeded, for each dataset served by ClimateData.ca or the CCCS website.  Proactive communication and regular mid-project data standards checks will ensure high quality data products and reduce the risk of potential late-stage data rejection.  Meeting or exceeding these standards will ensure that all new products distributed by the CCCS support the objective “to provide Canadians with information and support to consider climate change in their decisions”.

Where possible, the standards presented here align with broader national and international data standards initiatives.  This standards document itself is versioned according to [Semantic Versioning (semver)](semver.org) and version controlled using [Git](github.com).  Suggestions for new standards or modifications to the current standards are welcome and may be submitted via [Git pull requests](https://docs.github.com/en/free-pro-team@latest/github/collaborating-with-issues-and-pull-requests/about-pull-requests).

## Data Standards

### Documentation
The data must be associated with documentation that provides:
1. A clear, up-to-date, plain language executive summary that describes what the data tangibly represents.
1. A complete and up-to-date general and technical description that addresses the topic of each section of this data standards document, in detail.
1. At least one previous formal publication or report describing the methodology/data, or use of the methodology/data in a scientific or applied setting. 

### Relation to User Needs
The data must be associated with documentation that describes:
1. How the data itself, and/or specific delivery of the data on climatedata.ca or the CCCS website, addresses (in whole or in large part) a documented need of one or more Canadian user groups;
1. Why providing the data on ClimateData.ca or the CCCS website provides benefits relative to other existing datasets, or via delivery of the same data by other methods;
1. How the data:
   1.	Can be demonstrably applied to support user needs, or;
   1.	Requires further processing (e.g. via additional quantitative analysis or as use as input into an impacts model ).  If further processing is required, a description of the full processing workflow must be provided, along with a demonstration that this workflow is (or could in the near future) be feasible to undertake by all identified user groups. 
1. A specific case study/example that demonstrates how users have already used, or would use, the data.

### Scientific Integrity
The data must be associated with documentation that:
1. Provides scientific justification of methods used to develop the data.  It must include at a minimum:
   1. A comparison of the methods against other contemporary/similar methods and approaches
   1. An assessment of the methods against fundamental scientific theory and understanding;
   1. An objective critique of the strengths and weaknesses of the methods;
   1. An objective comparison to any/all similar methods/datasets.
1. Provides quantitative assessment of the resulting data.  This must include at a minimum: 
   1. For historical observations:
      1. Wherever possible, comparisons to independent observations or models to indicate measures of bias, particularly relative to the maximum bias that would be acceptable to users;
      1. Quantification of key data statistics, including (but not limited to) measures of averages, ranges, outliers, trends, and missing data;
   1. For future projections:
      1. Wherever possible, assessment of future values for realistic trends, ranges, and statistics;
      1. Comparison to any similar (‘apples-to-apples’) datasets;
1. Identifies an expert who is able to assist CCCS Support Desk with responses to data/methods queries, and/or train CCCS staff to a level that allows CCCS to confidently respond to these queries; 
1. Identifies one or more reviewers who could review, or already have reviewed, the data for scientific integrity. 

### Availability and Licensing
The data must be:
1. Free of cost;
1. Available for unrestricted use that meets current ClimateData/CCCS data distribution policies.  Data must be available for commercial use where commercial fees relate specifically to added value (e.g. reformatting/reorganizing/aggregation, advanced interpretation, integration into risk assessments, etc.) and not to data resale.  Licensing that meets this data standard requirement includes (but is not limited to) the [Creative Commons Attribution 4.0 International Public] License(https://creativecommons.org/licenses/by/4.0/legalcode), and for data produced by ECCC, the [License Agreement for Use of Environment and Climate Change Canada Data](https://climate.weather.gc.ca/prods_servs/attachment1_e.html).

### Provenance and Reproducibility
The data must be
1. Versioned using a consistent tracking protocol (e.g. [Semantic Versioning (semver)](semver.org) that identifies major/minor data revisions, for data versions hosted both at CCCS and elsewhere.  Enumerated data versions must be associated with at a minimum the following [World Meteorological Organization WMO-suggested items](https://library.wmo.int/doc_num.php?explnum_id=7867):
   1. The time at which the data was produced;
   1. Who (at the individual and organizational level) produced and is responsible for the data;
   1. What sources (e.g. models, observational instruments, etc.) the data was derived from;
   1. How/why the data changed relative to previous data versions (if applicable);
1. Reproducible through application of original underlying tools, including code, scripts, and/or documented workflows.  All tools must be made available to the portal partners upon request and be complete, version controlled and self-documented to the extent that a knowledgeable 3rd party (for example, an expert witness in a court proceeding) would not require additional information to reproduce a particular version of the data. 

### Data Coverage and Resolution 
The data must:
1. Cover the entire Canadian landmass or significant regions thereof, and/or coastal and offshore regions if required for maritime-specific user needs;
1. For gridded information: be at a spatial resolution that is directly applicable to identified user needs and, if feasible, be at the same resolution as existing climatedata.ca products;
1. Cover at a minimum:
   1. For climate models: the years 1950-2100 at a minimum;
   1. For observationally-sourced data: should cover at least 30 years and cover a period that is applicable to identified user needs;
1. Represent information at a temporal resolution that is directly applicable to identified user needs.

### Uncertainty Quantification
The data itself, or supporting datasets or documentation, must allow users to understand sources of uncertainty.  Depending on the data set, sources of uncertainty include:
1. Observations: for data derived from observations or data that indirectly incorporates observations (e.g. reanalysis data), the effect of uncertainties (e.g. observational bias and error, and measurement and methods uncertainties) should be qualitatively explained and if possible quantified;
1. Future projections: for data derived from climate model simulations, two sources of uncertainty should be addressed:
   1. Model uncertainty, via either: 
      1. a large ensemble of models in agreement with current multi-model project frameworks;
      1. an [objective model selection process](https://doi.org/10.1175/JCLI-D-14-00636.1);
   1. Scenario uncertainty: for data derived from climate model simulations, data should be provided that is consistent with as many of the following scenarios as possible:
      1. RCP2.6, RCP4.5, and RCP8.5 scenarios, or;
      1. SSP1-2.6, SSP2-4.5, SSP3-7.0, and SSP5-8.5 scenarios;
   1. Data derived using a single model initial-condition large ensemble (SMILE) must have information regarding how this ensemble captures multi-model and multi-scenario ensemble ranges.

### Metadata and Format  
Data metadata (information describing the data) must:
1. Conform to [Climate and Forecasting (CF) Conventions](https://cfconventions.org/) or other case-specific metadata standards that provide clear information on what the dataset represents.  Where data is meteorological or climatological and provided in netCDF format (preferred), full CF Convention compliance is required.  For other data formats, general CF Convention guidelines should be followed to all extents possible (for example, variable and data dimension names should use standard naming formats, even if these are captured via standardized file names).
1. Be in one of the following file formats:
   1. netCDF;
   1. text (CSV);
   1. GeoJSON;
   1. GeoTIFF;
   1. Shapefile;
1. Be associated with an accurate description of number of files and total dataset size (e.g. megabytes, gigabytes). 

### Quality Assurance/Quality Control Review
The data must be associated with certifying documentation:
1. Confirming that a quality assurance review has assessed that no errors are known to exist in the data creation methodology;
1. Confirming that a quality control review has assessed that no data errors and metadata errors are known to exist.

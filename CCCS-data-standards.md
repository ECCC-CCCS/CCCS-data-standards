# Canadian Centre for Climate Services Data Standards
## Summary and Objectives
Climate data is increasingly used to by users across Canada for consequential decisions around climate change risk, adaptation and resilience.  The Canadian Centre for Climate Services (CCCS) is a key developer and distributor of this data, and is therefore responsible for developing and maintaining accessible, transparent, trustworthy, and well-documented datasets.  To support this responsibility, this document defines a specific set of agreed-upon minimum, mandatory standards   for all new quantitative data  being developed for inclusion on ClimateData.ca and the CCCS website.  Barring exceptional circumstances, these standards must be met or exceeded for all data being considered for ClimateData.ca or the CCCS website, whether the data is developed by CCCS, federal, regional or provincial partners, academia, the private sector, or multi-stakeholder groups.  It is possible that different standards for a particular dataset could be addressed by a range of groups: for example, CCCS outreach/engagement staff may address user needs standards, academic partners may address scientific integrity standards, and CCCS technical partners may address metadata, provenance and reproducibility standards.  Ultimately, it is not so important who addresses each standard, so much as it is that each standard is ultimately met or exceeded, for each dataset served by ClimateData.ca or the CCCS website.
These standards – which where possible align with broader national and international data standards initiatives - should be proactively communicated to potential data partners well in advance of final data delivery to review working groups for consideration.  Proactive communication and regular mid-project data standards checks will ensure high quality data products and reduce the risk of potential late-stage data rejection.  Meeting or exceeding these standards will ensure that all new products distributed by the CCCS support the objective “to provide Canadians with information and support to consider climate change in their decisions”.
##Data Standards

### Documentation
The data must be associated with documentation that provides:
1. A clear, up-to-date, plain language executive summary that describes what the data tangibly represents.
2. A complete and up-to-date general and technical description that addresses the topic of each section of this data standards document, in detail.
3. At least one previous formal publication or report describing the methodology/data, or use of the methodology/data in a scientific or applied setting. 

### Relation to User Needs
The data must be associated with documentation that describes:
4.	How the data itself, and/or specific delivery of the data on climatedata.ca or the CCCS website, addresses (in whole or in large part) a documented need of one or more Canadian user groups;
5.	Why providing the data on ClimateData.ca or the CCCS website provides  benefits relative to other existing datasets, or via delivery of the same data by other methods;
6.	How the data:
**	Can be demonstrably applied to support user needs, or;
**	Requires further processing (e.g. via additional quantitative analysis or as use as input into an impacts model ).  If further processing is required, a description of the full processing workflow must be provided, along with a demonstration that this workflow is (or could in the near future) be feasible to undertake by all identified user groups. 
7	A specific case study/example that demonstrates how users have already used, or would use, the data.
3	Scientific Integrity
The data must be associated with documentation that:
8	Provides scientific justification of methods used to develop the data.  This cannot be a self-referential statement.  It must include at a minimum:
a.a	A comparison of the methods against other contemporary/similar methods and approaches
a.b	An assessment of the methods against fundamental scientific theory and understanding;
a.c	An objective critique of the strengths and weaknesses of the methods;
a.d	An objective comparison to any/all similar methods/datasets.
9	Provides quantitative assessment of the resulting data.  This must include at a minimum: 
a.a	For historical observations:
a.i	Wherever possible, comparisons to independent observations or models to indicate measures of bias, particularly relative to the maximum bias that would be acceptable to users;
a.ii	Quantification of key data statistics, including (but not limited to) measures of averages, ranges, outliers, trends, and missing data;
a.b	For future projections:
b.i	Wherever possible, assessment of future values for realistic trends, ranges, and statistics;
b.ii	Comparison to any similar (‘apples-to-apples’) datasets;
10	Identifies an expert who is prepared to assist CCCS Support Desk with responses to data/methods queries; 
11	Identifies one or more reviewers who could review, or already have reviewed, the data for scientific integrity. 
Availability and Licensing
The data must be:
12	Free ;
13	Available for unrestricted use that meets current ClimateData/CCCS data distribution policies.  Data must be available for commercial use where commercial fees relate specifically to added value (e.g.   advanced interpretation, integration into risk assessments, etc.) and not to data resale .   Licensing that meets this data standard requirement includes (but is not limited to) the Creative Commons Attribution 4.0 International Public License , and for data produced by ECCC, the License Agreement for Use of Environment and Climate Change Canada Data .
Provenance and Reproducibility
The data must be:
14	Versioned using a consistent tracking protocol that identifies all major/minor  data revisions, for data versions hosted both at CCCS and elsewhere.  Enumerated data versions must be associated with at a minimum the following :
a.a	The time at which the data was produced;
a.b	Who (at the individual and organizational level) produced and is responsible for the data;
a.c	What sources (e.g. models, observational instruments, etc.) the data was derived from;
a.d	How/why the data changed relative to previous data versions (if applicable).
15	Exactly reproducible  through application of original underlying tools, including codes , scripts, and/or documented workflows.  All tools must be made available to the portal partners upon request  and be complete, version controlled and self-documented to the extent that a knowledgeable 3rd party (for example, an expert witness in a court proceeding) would not require additional information to reproduce a particular version of the data. 
Data Coverage and Resolution 
The data must:
16	Cover the entire Canadian landmass   or significant regions thereof, and/or coastal and offshore regions if required for maritime-specific user needs. 
17	Represent information at a spatial resolution that is directly applicable to identified user needs and ideally be of the same resolution as existing climatedata.ca product  s.  
18	Cover at a minimum:
a.a	For climate models: the years 1950-2100 at a minimum;
a.b	For observationally-sourced data: should cover at least 30 years and cover a period that is applicable to identified user needs.
19	Represent information at a temporal resolution that is directly applicable to identified user needs.
Uncertainty Quantification
The data itself, or supporting datasets or documentation, must allow users to understand sources of uncertainty.  Depending on the data set, sources of uncertainty include:
20	Observations: for data derived from observations or data that indirectly incorporates observations (e.g. reanalysis data), the effect of uncertainties (e.g. observational bias and error, and measurement and methods uncertainties) should be qualitatively explained and if possible quantified.
21	Future projections: for data derived from climate model simulations, two sources of uncertainty should be addressed:
a.a	Model uncertainty: 
a.i	a large ensemble of models in agreement with current multi-model efforts;
a.ii	an objective model selection process .
a.b	Scenario uncertainty: for data derived from climate model simulations, data should be provided that is consistent with as many of the following scenarios as possible:
b.i	RCP2.6, RCP4.5, and RCP8.5 scenarios, or;
b.ii	SSP1-2.6, SSP2-4.5, SSP3-7.0, and SSP5-8.5 scenarios;
a.c	Data derived using a SMILE  ensemble must have information regarding how this ensemble captures multi-model and multi-scenario ensemble ranges.
Metadata and Format  
The data must:
22	Conform to Climate and Forecasting (CF) Conventions .  Where data is provided in netCDF format (preferred) , full CF Convention compliance is required  .   For other data formats, CF Convention guidelines must be followed to all extents possible (for example, variable and data dimension names should use CF Convention naming standards).
23	Be in one of the following file formats:
a.a	netCDF
a.b	text (CSV) 
a.c	GeoJSON
a.d	GeoTIFF
a.e	Shapefile
24	Be associated with an accurate description of number of files and total dataset volume. 
Quality Assurance/Quality Control Review
The data must be associated with certifying documentation:
25	Confirming that a quality assurance review has assessed that no errors exist  in the data creation methodology.
26	Confirming that a quality control review has assessed that no data errors and metadata errors exist .

Standards Document Lifecycle
This section is a bit long for a comment, so I’ve added it under change control.
It is almost certain that this document will need to be updated and maintained over time as experience accumulates. 
Please forgive me if you have already addressed these kinds of concerns.
1.	Establish a document version numbering system. Semver, as you propose for data itself, could serve.
2.	Place the document under version control, possibly somewhere central like GitHub.
3.	Encode the document in a way (e.g., Markdown) that makes it easy for people to propose and review revisions.
4.	Establish and document a change proposal and review process. This could be quite simple, but it’s advantageous to make it explicit.
5.	Publish the document from the repository to whatever other formats are desired.

<figure>
  <img src="logo-climate-data-ca-1-smaller.png" alt="logo" style="width:10%">
</figure>

# Canadian Centre for Climate Services Data Standards

# Version 0.0.2
La version française suit le texte anglais.
## Summary and Objectives
Climate data is increasingly used by users across Canada for consequential decisions around climate change risk, adaptation and resilience.  The [Canadian Centre for Climate Services (CCCS)](https://www.canada.ca/en/environment-climate-change/services/climate-change/canadian-centre-climate-services.html) is a key developer and distributor of this information, and it aims to develop and maintain accessible, transparent, trustworthy, and well-documented datasets.  To support this goal, this document defines a specific set of standards for all new quantitative data being developed for inclusion on ClimateData.ca and/or the CCCS website.  Barring exceptional circumstances, these standards must be met or exceeded for all data being considered for [ClimateData.ca](https://climatedata.ca/) or the [CCCS website](https://www.canada.ca/en/environment-climate-change/services/climate-change/canadian-centre-climate-services.html), whether the data is developed by CCCS, federal, regional or provincial partners, academia, the private sector, or multi-stakeholder groups.  Proactive communication and regular mid-project data standards checks will ensure high quality data products and reduce the risk of potential late-stage data rejection.  Meeting or exceeding these standards will ensure that all new products distributed by the CCCS support the objective “to provide Canadians with information and support to consider climate change in their decisions”.

Where possible, the standards presented here align with broader national and international data standards initiatives such as the [FAIR](https://www.go-fair.org/fair-principles/) principles. This standards document itself is versioned according to [Semantic Versioning (semver)](semver.org) and shared in a version controlled manner using [Git](github.com).  Suggestions for new standards or modifications to the current standards are welcome and may be submitted via [Git pull requests](https://docs.github.com/en/free-pro-team@latest/github/collaborating-with-issues-and-pull-requests/about-pull-requests).

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
   3. Should not be applied (e.g. potential user needs for which the data was not intended) 
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
3. Findable (Metadata and data should be easy to find for both humans and computers.)

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
      1. A large ensemble of models in agreement with current multi-model project frameworks;
      1. An [objective model selection process](https://doi.org/10.1175/JCLI-D-14-00636.1);
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


<figure>
  <img src="logo-climate-data-ca-1-smaller.png" alt="logo" style="width:10%">
</figure>

# Normes pour les données du Centre canadien des services climatiques

## Résumé et objectifs
Les données climatiques sont de plus en plus utilisées par les utilisateurs à travers le Canada pour prendre des décisions conséquentes concernant les risques liés aux changements climatiques, l'adaptation et la résilience.  Le [Centre canadien des services climatiques (CCSC)](https://www.canada.ca/fr/environnement-changement-climatique/services/changements-climatiques/centre-canadien-services-climatiques.html) est un développeur et un distributeur clé de cette information, et il vise à développer et à maintenir des ensembles de données accessibles, transparents, dignes de confiance et bien documentés.  Pour soutenir cet objectif, ce document définit un ensemble spécifique de normes pour toutes les nouvelles données quantitatives développées pour être incluses sur DonneesClimatiques.ca et/ou le site Web du CCSC.  Sauf circonstances exceptionnelles, ces normes doivent être respectées ou dépasser les attentes pour toutes les données envisagées pour [DonnesClimatiques.ca](https://donneesclimatiques.ca/) ou le [site Web du CCCS](https://www.canada.ca/fr/environnement-changement-climatique/services/changements-climatiques/centre-canadien-services-climatiques.html), que les données soient élaborées par le CCSC, des partenaires fédéraux, régionaux ou provinciaux, le milieu universitaire, le secteur privé ou des groupes multilatéraux.  Une communication proactive et des vérifications régulières des normes de données en milieu de projet assureront des produits de données de haute qualité et réduiront le risque de rejet potentiel des données à un stade avancé.  Le respect ou le dépassement des attentes de ces normes permettra d'assurer que tous les nouveaux produits distribués par le CCSC soutiennent l'objectif de " fournir aux Canadiens l'information et le soutien nécessaires pour prendre en compte le changement climatique dans leurs décisions ".

Dans la mesure du possible, les normes présentées ici s'alignent sur des initiatives nationales et internationales plus larges en matière de normes de données, comme les principes [FAIR](https://www.go-fair.org/fair-principles/). Le présent document de normes suivi la norme [Gestion sémantique de version (semver)](semver.org/lang/fr/) et il est partagé sous contrôle de version à l'aide de [Git](github.com).  Les suggestions de nouvelles normes ou de modifications des normes actuelles sont les bienvenues et peuvent être soumises via [À propos des demandes de tirage (pull requests)](https://docs.github.com/fr/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/about-pull-requests). 

## Standards de données

### Documentation
Les données doivent être associées à une documentation qui fournit :
1. Un résumé clair, à jour, en langage simple, qui décrit ce que les données représentent de manière tangible ; (*Obligatoire*)
2. Une description générale et technique complète et à jour qui aborde le sujet de chaque section de ce document de normes de données ; (*Obligatoire*)
3. Au moins une publication ou un rapport formel décrivant la méthodologie/les données, ou l'utilisation de la méthodologie/des données dans un cadre scientifique ou appliqué. (*Obligatoire*)
4. Au moins un document de référence en langage clair décrivant le contexte, les considérations et les processus clés (voir le point 3 sur la relation avec les besoins des utilisateurs) relatifs à ces données. (*Obligatoire*)  

### Relation avec les besoins des utilisateurs
Les données doivent être associées à une documentation qui décrit :
1. Comment les données elles-mêmes, et/ou la livraison spécifique des données sur DonneesClimatiques.ca ou le site Web de la CCSC, répondent (en totalité ou en grande partie) à un besoin documenté d'un ou de plusieurs groupes d'utilisateurs canadiens ; (*Obligatoire*)
2. Pourquoi la fourniture des données sur DonneesClimatiques.ca ou sur le site Web de la CCSC présente des avantages par rapport à d'autres ensembles de données existants ou à la fourniture des mêmes données par d'autres méthodes ; (*Recommandé*).
3. Comment les données : (*Obligatoire*)
   1.	Peuvent être appliquées de manière démontrable pour répondre aux besoins des utilisateurs, ou ;
   2.	Nécessitent un traitement supplémentaire (par exemple, via une analyse quantitative supplémentaire ou en tant qu'entrée dans un modèle d'impact).  Si un traitement supplémentaire est nécessaire, une description du flux de travail complet du traitement doit être fournie, ainsi qu'une démonstration que ce flux de travail est (ou pourrait dans un avenir proche) être réalisable par tous les groupes d'utilisateurs identifiés.    
   3. Ne devraient pas être appliquées (par exemple, les besoins potentiels des utilisateurs pour lesquels les données n'ont pas été prévues) 
4. Une étude de cas/un exemple spécifique qui démontre comment les utilisateurs ont déjà utilisé, ou utiliseraient, les données. (*Recommandé*)

### Intégrité scientifique
Les données doivent être associées à une documentation (ou des références à une documentation antérieure) qui :
1. Fournit une justification scientifique des méthodes utilisées pour développer les données.  Elle doit comprendre au minimum : (*Obligatoire*)
   1. Un examen qualitatif des méthodes par rapport à d'autres méthodes et approches contemporaines/similaires ;
   2. Une évaluation des méthodes par rapport à la théorie et à la compréhension scientifiques fondamentales ;
   3. Une critique objective des forces et faiblesses des méthodes ; 
2. Fournit une évaluation quantitative des données résultantes.  Cela doit inclure :  (*Obligatoire*)
   1. Pour les données basées sur des observations historiques :
      1. Chaque fois que cela est possible et faisable, des comparaisons avec des observations ou des modèles indépendants pour indiquer les mesures de biais, en particulier par rapport au biais maximal qui serait acceptable pour les utilisateurs ;
      2. La quantification des statistiques clés des données, y compris (mais sans s'y limiter) les mesures des moyennes, des fourchettes, des valeurs aberrantes, des tendances et des données manquantes ;
   2. Pour les projections futures :  
      1. Dans la mesure du possible, évaluation des valeurs futures pour des tendances, des fourchettes et des statistiques réalistes ;
      2. Comparaison avec des ensembles de données similaires ("pommes à pommes") ;
3. Décrit un accord pour que les développeurs de données fournissent au besoin un soutien et/ou une formation au personnel du centre d'aide du CCSC pour répondre aux demandes de données/méthodes ; (*Recommandé*).
4. Identifie un ou plusieurs examinateurs qui pourraient examiner, ou ont déjà examiné, les données pour en vérifier l'intégrité scientifique. (*Recommandé*)

### Disponibilité et licence
Les données doivent être :
1. Gratuites ; (*Obligatoire*)
2. Disponibles pour une utilisation sans restriction, conformément aux [politiques de distribution des données et licences de DonnéesClimatiques.ca/CCSC](https://donneesclimatiques.ca/legal-fr/).  Les données doivent être disponibles pour une utilisation commerciale lorsque les frais commerciaux sont spécifiquement liés à la valeur ajoutée (par exemple, reformatage/réorganisation/agrégation, interprétation avancée, intégration dans les évaluations des risques, etc.  Les licences qui répondent à cette exigence de norme de données comprennent (sans s'y limiter) la [Licence publique Creative Commons Attribution 4.0 International](https://creativecommons.org/licenses/by/4.0/legalcode.fr), et pour les données produites par l'ECCC, le [Contrat de licence pour l'utilisation des données d'Environnement et Changement climatique Canada](https://climat.meteo.gc.ca/prods_servs/attachment1_f.html) et la [Licence du gouvernement ouvert – Canada](https://ouvert.canada.ca/fr/licence-du-gouvernement-ouvert-canada). (*Obligatoire*)
3. Trouvable (Les métadonnées et les données doivent être faciles à trouver, tant pour les humains que pour les ordinateurs). (*Obligatoire*)

### Provenance et reproductibilité
Les données doivent être :
1. Versionnées à l'aide d'un protocole de suivi cohérent (par exemple [Gestion sémantique de version (semver)](semver.org/lang/fr/) qui identifie les révisions majeures et mineures des données, pour les versions de données hébergées au CCCS et ailleurs.  Les versions de données énumérées doivent être associées aux [éléments suivants suggérés par l'Organisation météorologique mondiale (OMM)](https://library.wmo.int/doc_num.php?explnum_id=7867): (*Obligatoire*)
   1. L'heure à laquelle les données ont été produites ;
   2. Qui (au niveau individuel et organisationnel) a produit et est responsable des données ;
   3. De quelles sources (par exemple, modèles, instruments d'observation, etc.) les données ont été dérivées ;
   4. Comment/pourquoi les données ont changé par rapport aux versions précédentes des données (le cas échéant) ;
2. Reproductible par l'application des outils sous-jacents originaux, y compris le code, les scripts, et/ou les flux de travail documentés.  Tous les outils doivent être mis à la disposition des partenaires du portail sur demande et être complets, contrôlés par version et auto-documentés de manière à ce qu'une tierce partie bien informée (par exemple, un témoin expert dans une procédure judiciaire) n'ait pas besoin d'informations supplémentaires pour reproduire une version particulière des données. (*Recommandé*)

### Couverture et résolution des données 
Les données doivent :
1. Couvrir l'ensemble de la masse continentale du Canada ou des régions importantes de celle-ci, et/ou les régions côtières et extracôtières si cela est nécessaire pour les besoins spécifiques des utilisateurs maritimes ; (*Obligatoire*)
2. Pour les données maillées : être à une résolution spatiale directement applicable aux besoins identifiés des utilisateurs et, si possible, être à la même résolution que les produits existants de DonneesClimatiques.ca ; (*Obligatoire*) 3.
4. Couvrir au minimum : (*Obligatoire*)
   1. Pour les modèles climatiques : les années 1950-2100 au minimum ;
   2. Pour les données issues des observations : ils devraient couvrir au moins 30 ans et couvrir une période qui est applicable aux besoins identifiés des utilisateurs ;
5. Représenter les informations à une résolution temporelle qui est directement applicable aux besoins identifiés des utilisateurs. (*Obligatoire*)

### Quantification des incertitudes
Les données elles-mêmes, ou les ensembles de données ou la documentation à l'appui doivent permettre au personnel et aux utilisateurs du CCSC de comprendre les sources d'incertitude.  L'"incertitude" peut prendre différentes formes selon les données en question.  En fonction de l'ensemble des données, les sources d'incertitude qui devraient être abordées pourraient inclure :
1. Observations : pour les données dérivées d'observations ou les données qui incorporent indirectement des observations (par exemple, les données de réanalyse), l'effet des incertitudes (par exemple, le biais et l'erreur d'observation, l'incertitude dans les méthodes de traitement des données) devrait être expliqué qualitativement et si possible quantifié ; (*Obligatoire*)
2. Projections futures : pour les données dérivées de simulations de modèles climatiques, trois sources d'incertitude doivent être abordées : (*Obligatoire*)
   1. L'incertitude du modèle, via soit : 
      1. Un grand ensemble de modèles en accord avec les cadres actuels des projets multi-modèles ;
      1. Un [processus objectif de sélection des modèles](https://doi.org/10.1175/JCLI-D-14-00636.1) ;
   2. Incertitude du scénario : pour les données dérivées de simulations de modèles climatiques, il convient de fournir des données distinctes du scénario qui sont cohérentes avec le plus grand nombre possible des scénarios suivants :
      1. Scénarios RCP2.6, RCP4.5, et RCP8.5, ou ;
      1. Scénarios SSP1-2.6, SSP2-4.5, SSP3-7.0, et SSP5-8.5 ;
   3. L'incertitude de la variabilité interne, via des simulations d'ensemble ou d'autres approches équivalentes.

### Métadonnées  
Les métadonnées des données (informations décrivant les données) doivent : 
1. Se conformer aux [Conventions sur le climat et la prévision (CF)](https://cfconventions.org/) ou à d'autres normes de métadonnées spécifiques qui fournissent des informations claires sur ce que représente le jeu de données.  Lorsque les données sont météorologiques ou climatologiques et fournies en format netCDF (de préférence), la conformité aux conventions CF est recommandée comme norme minimale.  Pour les autres formats de données, les lignes directrices générales de la Convention CF en matière de métadonnées doivent être suivies dans toute la mesure du possible (par exemple, les noms des variables et des dimensions des données doivent utiliser des formats de dénomination standard, même s'ils sont saisis par le biais de conventions de dénomination de fichiers standardisées) ; (*Obligatoire*).
2. Dans la mesure du possible, exploitez les capacités de métadonnées des formats de fichiers pour intégrer les métadonnées dans les fichiers de données eux-mêmes.
3. Être associés à une description précise du nombre de fichiers et de la taille totale de l'ensemble de données (p. ex. mégabytes, gigabytes) ; (*Obligatoire*)
4. Inclure des informations relatives à : (*Obligatoire*)
   1. La licence ;
   2. La provenance

### Format du fichier
1. Être dans l'un des formats de fichier suivants : (*Recommandé*)
   1. netCDF ;
   2. texte (CSV) ;
   3. GeoJSON ;
   4. GeoTIFF ;
   5. Shapefile ;

### Examen de l'assurance qualité/contrôle de la qualité
Les données doivent être associées à une documentation certifiée :
1. Confirmant qu'un examen d'assurance de la qualité a évalué qu'aucune erreur n'est connue dans la méthodologie de création des données ; (*Obligatoire*)
2. Confirmant qu'un examen du contrôle de la qualité a permis d'évaluer qu'aucune erreur n'est connue dans les données et métadonnées finales. (*Obligatoire*)

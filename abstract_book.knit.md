---
title: "abstract_book"
author: "Peter Higgins"
date: "8/24/2021"
output: html_document
---



## Abstract Book for R/Medicine 2021



```
Presenters: Karandeep Singh 
Presentation Type: Keynote Address 
Presentation: O1 
Title: Bringing Machine Learning Models to the Bedside at Scale 
 Abstract: Early warning systems -- machine learning (ML) models that run every few minutes on hospitalized patients -- have the potential to play a large role in supporting patient care. By estimating the risk of a myriad of clinical outcomes using realtime data, such systems identify patients in need of attention even when clinicians are not in the room. When linked to interventions, these models bring care to patients when they need it most. However, deploying model-driven systems in a hospital environment at scale comes with several challenges related to software infrastructure and governance in addition to model-related issues (e.g., miscalibration, selection of relevant thresholds, and use of proprietary models) and intervention-related issues (e.g., alert fatigue, assessing efficacy). In this talk, I will share several examples of real-world issues faced by health systems related to deploying ML models at scale and in bringing them to the bedside. I will demonstrate how R has played in role in the evaluation of ML models at the University of Michigan. I will draw from my own experience, where I oversee the operationalization of ML models at Michigan Medicine, as well as that from colleagues across the country. 

Presenters: Julia Romanowska 
Presentation Type: Lightning Talk 
Presentation: O2 
Title: Diving into Registry Data: Using R for Large Norwegian Health Registries 
 Abstract: Traditional process of designing new drug is timely, costly (https://en.wikipedia.org/wiki/Cost_of_drug_development), and often fails (https://en.wikipedia.org/wiki/Drug_development#Clinical_phase). However, by analyzing the usage patterns of the drugs already on the market, alongside the history of illnesses of each person, new drug application areas might be discovered - so-called drug repurposing.
In Norway, national registries have been collecting various types of data on each Norwegian citizen for many decades. Within our project, (Drug Repurposing for NEurological diseases, http://link.uib.no/drone), we have access to the entire Prescription Registry, along with selected diagnoses from Patient Registry, and demographic data from Statistics Norway. This huge amount of information requires appropriate programming approaches so that the full potential of the datasets is harnessed. We have chosen R, with its vast number of packages and ease of coding, to implement advanced methods of epidemiology, bioinformatics, and machine learning to find new drugs for neurological diseases. I will briefly present our research method and point to several R packages and techniques we are using to make our work reproducible and effective. 

Presenters: Layla Bouzoubaa 
Presentation Type: Lightning Talk 
Presentation: O3 
Title: {DOPE}: An R Package for Processing & Classifying Drug Names 
 Abstract: DOPE (Drug Ontology Parsing Engine) is an R package that aims to synthesize and harmonize drug names from multiple sources, allowing researchers to look up drugs by "brand", "generic" or "street" names.
DOPE has built a lexicon with drug names grouped into 11 categories (i.e.,
stimulants, depressants, designer drugs, etc.) and 41 classes (e.g., amphetamines, cocaine, etc.) based on categorization provided by the DEA and synonyms/slang provided on publicly available websites. 
It contains the datasets and a function needed to parse a set of potential drug names and classify them by their class and type. The functions automatically classify any sets of words, which can be a mixture of slang or formal names. A summary function provides summaries when a drug type/class is ambiguous or if a substance is a combination of multiple drugs (i.e., speedball).DOPE can be the backbone for future data science projects, allowing people to efficiently collect
and synthesize drug data while dealing with ambiguous terms. For example, DOPE can be used during data collection to prompt clarification for uncommon slang that the DEA has identified, such as "cheese", which can refer to heroin, marijuana or methamphetamine. 

Presenters: Ethan Heinzen, Beth Atkinson, Jason Sinnwell 
Presentation Type: Regular Talk 
Presentation: O4 
Title: An Arsenal of R Functions for Statistical Summaries 
 Abstract: arsenal is an R package designed to make statistical summaries easy.  It includes many functions which the user will find useful to have in his/her "arsenal" of functions.  There are 6 main functions, each of which is motivated by a SAS procedure or local macro of similar functionality.
Its reporting capabilities are streamlined to work within the latest reporting tools in R and RStudio and use formulas and versatile summary statistics for tables and models. The primary functions include tableby(), a Table-1-like summary of multiple variable types 'by' the levels of one or more categorical variables; paired(), a Table-1-like summary of multiple variable types paired across two time points; modelsum(), which performs simple model fits on one or more endpoints for many variables (univariate or adjusted for covariates); freqlist(), a powerful frequency table across many categorical variables; comparedf(), a function for comparing data.frames; and write2(), a function to output tables to a document.
 

Presenters: Robert Lobato 
Presentation Type: Lightning Talk 
Presentation: O5 
Title: R and Shiny Dashboards Facilitate Quality Improvement in Anesthesiology and Perioperative Care 
 Abstract: Quality improvement studies quantify progress made toward implementing evidence-based guidelines into clinical care. The Department of Anesthesiology at the University of Nebraska Medical Center developed a dashboard using R and Shiny to track several perioperative quality metrics developed by the Centers for Medicare and Medicaid Services. Despite high performance on a quality measure evaluating rates of postoperative nausea and vomiting (PONV) in high-risk patients, we continued to observe unacceptably high rates of PONV after surgery. A reanalysis of patient-level data identified subsets of patients, not included in the high-risk group addressed in CMS metrics, who were being under-treated according to current perioperative society guidelines. An improvement was made to our Shiny dashboard to place more emphasis on deviations from guidelines-based perioperative care and the resulting rates of complications in those patients. This quality improvement study demonstrates the utility of R and Shiny dashboards in identifying areas where patient care deviates from evidence-based guidelines and illustrates the importance of quality improvement in guiding clinical practice. 

Presenters: Francisco Requena 
Presentation Type: Lightning Talk 
Presentation: O6 
Title: Building an interpretable machine learning model API for the clinical interpretation of CNVs in patients with rare diseases 
 Abstract: Copy number variants (CNVs) play an important role in many rare diseases. Despite their relevance, the clinical interpretation of CNVs is challenging and time-consuming. Moreover, current NGS technologies report a median of 7,439 structural variants per genome, making tool development more urgent.

To address this problem, we developed CNVscore, a machine learning (ML) approach designed to aid in the clinical interpretation of CNVs. To build CNVscore, we used the R package rtemis to train a rule-based model (RuleFit) and rstanarm to create a Bayesian model. We combined these two approaches (rule-based and Bayesian) to create an interpretable model capable of quantifying the uncertainty level for each prediction. This approach achieved performance comparable to popular ML models (e.g. XGboost, random forest) while allowing the clinician to know which rules were used to make the prediction and the degree of confidence the model has in that prediction.

To make CNVscore easily accessible, we deployed it as an API with the package plumber. In addition, the API will be integrated into our recently published Shiny tool CNVxplorer  (http://cnvxplorer.com) so that the user can evaluate the model predictions with complementary information. 

Presenters: Timothy Keyes 
Presentation Type: Regular Talk 
Presentation: O7 
Title: {tidyTOF}: Building a reproducible pipeline to predict patient outcomes from single-cell data using tidy data principles 
 Abstract: In recent years, the concept of “tidiness”—a data analysis framework in which data frames are structured such that each variable is a column and each observation is a row—has become a staple of the R community. This is largely because working with “tidy data” makes it easy to map the meaning of a dataset to a specific and consistent structure, which in turn allows for the development of easily-used data analysis tools for a variety of applications. Despite these strengths, relatively few tools have been developed for analyzing clinical and biomedical data using tidy data principles.

Here, we present {tidytof} – a novel R package for tidy analysis of mass cytometry (CyTOF) single-cell data – as a case study for using tidy data principles to simplify the manipulation, visualization, and modeling of biomedical data. Specifically, {tidytof} leverages tidy data analysis to implement a reproducible and human-readable pipeline for common single-cell analysis tasks including reading/writing data, clustering, dimensionality reduction, feature engineering, and patient-outcomes modeling. Our presentation will highlight the process behind and benefits of using tidy principles to build simple and intuitive biomedical data analysis workflows. 

Presenters: David Miller, Sophia Shalhout 
Presentation Type: Regular Talk 
Presentation: O8 
Title: GENETEX - A GENomics Report TEXt Mining R Package and Shiny Application Designed to Capture Real-World Clinico-Genomic Data 
 Abstract: Objectives: Clinico-Genomic Data (CGD) acquired through routine clinical practice has the potential to improve our understanding of clinical oncology. However, these data often reside in heterogeneous and semi-structured data, resulting in prolonged time-to-analyses.
Materials and Methods: We created GENETEX: an R package and Shiny application for text mining genomic reports from EHR and direct import into REDCap.
Results: GENETEX facilitates the abstraction of CGD from EHR and streamlines capture of structured data into REDCap. Its functions include natural language processing of key genomic information, transformation of semi-structured data into structured data and importation into REDCap. When evaluated with manual abstraction, GENETEX had >99% agreement and captured CGD in approximately one-fifth the time.
Conclusions: GENETEX is freely available under the Massachusetts Institute of Technology license and can be obtained from GitHub. GENETEX is executed in R and deployed as a Shiny application for non-R users. It produces high-fidelity abstraction of CGD in a fraction of the time. 

Presenters: Luke McGuinness, Randall Boyes, Alex Fowler 
Presentation Type: Lightning Talk 
Presentation: O9 
Title: Incorporating risk-of-bias assessments into evidence syntheses with robvis 
 Abstract: Risk-of-bias assessment is regularly hailed as an essential part of the evidence synthesis process, providing a structured way to critically assess the internal validity of included studies. However, evidence from meta-research studies has demonstrated that while risk-of-bias assessments are performed, the data produced by the assessments are infrequently visualised or incorporated into statistical analyses. 

{robvis} is an established R package which aims to solve this issue by making it easier for reseachers to create reproducible publication-quality risk-of-bias plots in line with best-practice guidelines. This presentation for R Medicine will introduce the robvis package, outline the motivation for its development, and showcase how users can use the package to report risk-of-bias assessments in their own reviews. It will also introduce new functionality in robvis, focused on better integration with the {metafor} package for performing meta-analysis, which allows users both to present statistical analyses and risk-of-bias results side-by-side (via graphics known as "paired forest plots") and to readily stratify their analysis by the level of risk of bias in each included study as part of a sensitivity analysis. 

Presenters: Christian Röver 
Presentation Type: Regular Talk 
Presentation: O10 
Title: Bayesian random-effects meta-analysis using bayesmeta 
 Abstract: Meta analyses are useful in many medical fields.  A Bayesian approach to inference is very attractive in this context, especially when a meta-analysis is based only on few studies.  The bayesmeta R package provides readily accessible tools to perform Bayesian meta-analyses and generate plots and summaries, without having to worry about computational details.  It allows for flexible prior specification and instant access to the resulting posterior distributions, including prediction and shrinkage estimation, and facilitating for example quick sensitivity checks.  This presentation will showcase its use and also provide pointers to more advanced applications. 

Presenters: Sean Meyer, Karandeep Singh 
Presentation Type: Lightning Talk 
Presentation: O11 
Title: gpmodels: A Grammar of Prediction Models 
 Abstract: The gpmodels R package provides a grammar for data preparation and evaluation of fixed-origin and rolling-origin prediction models using data collected at irregular intervals (e.g., electronic health record data). Since predictions often begin and end at specific times for each patient (e.g., hospital admission or discharge), gpmodels provides clean, pipeable functions for the creation of predictors and outcomes that are linked to either a fixed origin (e.g., single observation per patient) or rolling origin (e.g., multiple observations per patient). Creation of machine learning-ready is highly CPU- and memory-intensive, so gpmodels supports parallel processing (using furrr), allows processing individual chunks in parallel, and can write output directly to file to minimize memory usage. gpmodels also provides functions to preprocess data elements (e.g., dummy coding of time-series factor variables) and for the evaluation of time-series models. The model evaluation code in gpmodels is based on the code used in recent publications evaluating performance of the Epic Sepsis Model and the Epic Deterioration Index. 

Presenters: Beth Atkinson 
Presentation Type: Regular Talk 
Presentation: O12 
Title: Multistate data using the survival package 
 Abstract: Survival data, also known as time-to-event data, is very common in medical research. Historically, analysis focused on single endpoints such as death or cancer recurrence. Increasingly, research questions are more complex and need multistate transition models.  This approach allows you to handle situations where subjects move between states, such as healthy to illness to death. The survival package has had functions to handle standard survival analysis for many years. Starting with version 3.2 there are tools to handle multistate models as well.  The overall goals for the additions to the packages were to: 
* Make probability-in-state curves as easy to create as a Kaplan-Meier curve 
* Make multistate models as easy to fit as a Cox model
* Provide access to other estimates of absolute risk, e.g., the restricted mean time in state.

This presentation will highlight questions that can be addressed with multistate models and will show how to code analyses to answer the questions. 

Presenters: Ariel Mundo 
Presentation Type: Lightning Talk 
Presentation: O13 
Title: Generalized additive models for longitudinal biomedical data 
 Abstract: Biomedical research frequently uses longitudinal studies to capture the evolution of an effect over time. Traditionally, such data is analyzed using repeated measures ANOVA (rm-ANOVA) models or linear mixed models (LMEM; but it is frequently the case that those models are not appropriate because the trend of the data is not linear. This non-linear behavior in longitudinal data occurs frequently in biomedical research, but its implications from a Statistical perspective are often not considered, leading to unreliable inference.
Generalized additive models (GAMs) are a class of models that allow non-linear trends in the data and that can provide robust inference, but they are little known in the biomedical realm. 

This talk will provide a brief summary of examples in the biomedical literature where non-linear trends in data have been observed, some of the limitations of linear models that make them unusable in non-linear data, and will show a brief implementation of GAMs using R in simulated data that follows reported trends in the literature. 

Presenters: Victor Castro, Roy Perlis 
Presentation Type: Regular Talk 
Presentation: O14 
Title: Assessing Machine Learning Model Performance in Diverse Populations and Across Time 
 Abstract: In recent years numerous machine learning models to predict clinical risk have been reported in the research literature.  Many of these models are developed in large and diverse databases of electronic health record or other medical datasets.  Few risk models, however, have been evaluated for potential bias among subgroups of patients in the training or evaluation set.  In this talk we’ll cover our experience training a model to stratify risk among patients hospitalized for COVID-19 during the early course of the pandemic and then performing subsequent evaluation of the model performance a year later.  We’ll describe how we extend the tidymodels yardstick package to evaluate performance across time as well as subgroups of patients.  Our results illustrate the importance of investigating risk stratification models across patient subgroups, as a step toward ensuring that particular groups of patients are not adversely impacted by the application of machine learning models in healthcare. 

Presenters: Jie Cao, Karandeep Singh 
Presentation Type: Lightning Talk 
Presentation: O15 
Title: runway: An R Package to Visualize Prediction Model Performance 
 Abstract: Runway is an R package that facilitates the visual evaluation and comparison of prediction models and provides publication-ready graphics. Visualizing performance is an important way to communicate a prediction model’s strengths and limitations. The core visualizations implemented in runway are threshold-performance plots, calibration plots, and receiver operating characteristic (ROC) curves. Threshold-performance plots provide a clean, faceted approach to demonstrating sensitivities, specificities, and positive and negative predictive values across a range of probability thresholds. Calibration curves show either binned (e.g., deciles) or continuous measures of observed risk across a range of predicted risk. Models with different types of miscalibration can be difficult to compare on a threshold-performance plot, so the package also supports traditional ROC curves. The visualizations include 95% confidence intervals, can be used to plot either a single model (black and white) or multiple models (in color), and include distributions of predicted risk (as histograms for single models and density plots for multiple models). 

Presenters: Andreas Soteriades, Chris Beeley 
Presentation Type: Regular Talk 
Presentation: O16 
Title: Scaling up: Deployable Shiny and Text Mining to Guide Decision-Making in the Healthcare Sector of an Entire Country 
 Abstract: Undoubtedly, R is a powerful tool for data manipulation and visualization, statistical analysis, and machine learning (ML). Shiny is excellent for producing dashboards, and so are “tidymodels” and “mlr3” for building ML pipelines. However, Shiny developers often come across situations where the code for a complicated Shiny app becomes massive, hard to read, understand and debug, and it is so tailored to the dataset that the app cannot work as a framework for other datasets. Similarly, ML practitioners often face the fact that R simply cannot handle efficiently large ML pipelines and datasets. In this talk, we will discuss how we built and deployed a scalable and robust text classification pipeline and dashboard using the R packages “Golem” and “reticulate”. Golem helps build and ship Shiny apps as R packages that are modular, agnostic to deployment and submission-ready (performs tests automatically). Package “reticulate” allows running Python through R, which gave us access to the state-of-the-art Scikit-learn Python library for ML. We will show how we successfully used both packages to develop a tool for England’s National Health Service. 

Presenters: Richard Hanna, Stephan Kadauke 
Presentation Type: Lightning Talk 
Presentation: O17 
Title: Stem Cell Transplant Outcomes Reporting using R/Shiny 
 Abstract: Stem cell transplantation is a life-saving therapy for various malignant and non-malignant diseases. To aggregate real-world data on transplant patients, all cancer centers in the U.S. are required by law to report outcomes such as the time from transplant to the emergence of certain blood cells, known as “engraftment.”

Traditionally, engraftment is reported by data managers who manually look up information in medical records and complete web-based forms. This tedious manual process requires integration of multiple data sources and, at a top-tier pediatric cancer center, was found to have error rates as high as 25%.

To mitigate this problem, we developed an R/Shiny application that calculates engraftment dates by querying and integrating multiple clinical data sources. We used the {golem} framework and deployed the app on RStudio Connect. The app passed clinical validation and is now in day-to-day use by our data managers, having eliminated the manual process.

In this lightning talk, we will outline the clinical validation, production engineering, and operationalization of the engraftment app. We will also discuss how the app could be implemented at other cancer centers. 

Presenters: Michael Kane 
Presentation Type: Regular Talk 
Presentation: O18 
Title: Collaborative, Reproducible Exploration of Clinical Trial Data 
 Abstract: Clinical trial data, recorded as ADaM (or ADaM-like) data, attempts to capture all measurements made during a clinical trial that may be used to assess patient prognosis and the predictive relationships between a therapy and a set of outcomes. Biostatisticians’ whose job is to analyze these types of data collaborate with clinicians to understand the data through tables, visualizations, and preliminary analyses. Even though these data are structured they may still be complex and require iteration between biostatisticians and the clinicians with whom they are collaborating. In this talk, we will show how several R packages can be used in conjunction to create more comprehensive exploration to reduce this iteration. The approach has users assign roles to variables and then automates the process of generating summaries of the bivariate relationships between variables in specified roles. These summaries can then be displayed in a navigable, interactive html environment that can be disseminated to all members of a collaboration for review and discussion. We will provide several examples of these reports and show how they can be extended to include analyses thereby encapsulating all stages of the data analysis. 

Presenters: Judith Lewis, Stephany Duda 
Presentation Type: Regular Talk 
Presentation: O19 
Title: R/Shiny and REDCap: Streamlining Data Workflow in a Global Research Consortium 
 Abstract: We will describe the design and impact of a web-based R/Shiny/RMarkdown application that provides a data harmonization workflow for large observational research consortia. This cloud-based application has an advanced Shiny UI and is integrated with REDCap via the R httr package. Users can upload datasets to check data quality, generate reports, visualize data, and securely transfer files.  Details about the expected format of the data (tables, variables, formats, valid codes for coded variables defined in the data model) are stored in REDCap and accessed via the R/REDCap API. The application uses these details to auto-generate data quality checks and generate customizable PDF reports for download. User authentication, file transfer information, and audit trails are also exchanged with REDCap.
One year after the tool was launched in an international HIV research consortium, users reported that the data quality feedback, reproducible reports, and easy-to-use workflow of the Harmonist Data Toolkit helped them improve data quality and decreased the amount of time required for data preparation and reporting. The Toolkit is designed to be adapted for use by other research networks. 

Presenters: Laura Wiley, David Mayer 
Presentation Type: Regular Talk 
Presentation: O20 
Title: {ReviewR}: A Shiny App for Reviewing Clinical Records 
 Abstract: Reviewing clinical records is essential for data extraction and validating algorithms. Traditionally, researchers review the electronic health record (e.g., Epic, Cerner) and record abstractions in spreadsheets (e.g., Excel). However, this has workflow challenges (multiple windows, copy/pasting wrong patient identifiers, etc.), and increasingly organizations are limiting EHR access for non-clinical researchers. To solve these challenges, we created ReviewR, a Shiny application that combines the display of patient records from clinical data warehouses with an abstraction interface to improve workflow and review accuracy. ReviewR is architected to be flexible across clinical data models (OMOP, MIMIC-II) and databases (Google BigQuery, Postgres). We include functions to help users extend ReviewR to support custom data models and databases as needed. Chart view functionality is supported by the DT package, allowing each table to be filtered by multiple columns and text searching, filtering, and highlighting. The chart abstraction interface allows for multiple types of data capture (e.g., radio buttons, check lists, free text entry, etc.) uploaded securely to the research data management system REDCap. ReviewR is available on CRAN. 

Presenters: Ziad Obermeyer 
Presentation Type: Keynote Address 
Presentation: O21 
Title: Dissecting Algorithmic Bias 
 Abstract: Algorithmic bias is everywhere. Our work with dozens of organizations—health care providers, insurers, technology companies, and regulators—has taught us that biased algorithms are deployed throughout the health care system, influencing clinical care, operational workflows, and policy. 

Presenters: Jie Cao, Karandeep Singh 
Presentation Type: Regular Talk 
Presentation: O22 
Title: clinspacy: An R Package for Clinical Natural Language Processing 
 Abstract: Clinical text contains rich information that is potentially powerful input for machine learning in medicine. However, natural language processing (NLP) tools used to process clinical text need to be tailored to the clinical context. Building on Python’s spaCy framework, scispaCy’s clinical language model and Unified Medical Language System (UMLS) concept mapping, and medspaCy’s context and sectionizer tools, clinspacy provides a single-function capability to process massive volumes of clinical text directly to a data frame or a CSV file.

Although clinspacy depends upon Python, users do not need to install it manually. The package automatically detects and installs miniconda and all dependencies. Beyond providing an interface to the aforementioned Python packages, clinspacy also enables the creation of model-ready datasets through its bind_*() functions that can be used to create bag-of-entities, bag-of-concepts, and concept-embedding datasets leveraging either scispaCy or cui2vec embeddings. clinspacy is available on GitHub and CRAN. 

Presenters: Peter Higgins 
Presentation Type: Lightning Talk 
Presentation: O23 
Title: Using the {medicaldata} package for teaching #rstats 
 Abstract: It can be difficult to find good datasets for teaching medical research. Many are proprietary or hidden behind privacy concerns. But learners really appreciate working with real medical data, particularly from clinical trials. I have gathered together several datasets, reconstructed others, and received some lovely donations of deidentified data sets.

These have been packaged into the {medicaldata} package, which is available on Github, and if I am especially stubborn and persistent, possibly soon on CRAN. This package includes several well-documented datasets, from as early as 1757 (James Lind and scurvy) to 2020 (COVID testing). Several of the clinical trials were ones I was involved with, and others were reconstructed from tables (Streptomycin for Pulmonary TB). 
This package can be a helpful teaching resource, as the datasets are carefully documented, with explanations and codebooks, both in the help files and online with links to pdf documents on each dataset in the Github repo at https://github.com/higgi13425/medicaldata. 
This package functions as a companion to the e-book Reproducible Medical Research with R, but can be used independently. https://bookdown.org/pdr_higgins/rmrwr/. 

Presenters: Travis Gerke 
Presentation Type: Regular Talk 
Presentation: O24 
Title: CONSORT diagrams in R with {ggconsort} 
 Abstract: CONSORT diagrams are the industry standard graphic for representing participant flow in a clinical trial. Several teams have considered R packages for CONSORT diagram construction, but have fallen short of end-to-end automation. Most notably, Dr. Peter Higgins proposed an excellent CONSORT design overview in his R/Medicine 2020 talk, in which he described the legacy diagram construction as "an artisanal product built by counting categories, then copy and pasting results into templates." Here, I will present a fresh look at the {ggconsort} package, which embraces aspects of CONSORT construction that are inherently artisanal, but eliminates error-prone manual entry. Specifically, I segment CONSORT creation into two stages: (1) CONSORT annotation capture at the time of data wrangling, and (2) diagram layout. I will demonstrate how stage (1) can be built into a single tidyverse chain. Stage (2) maintains some artisanal aspects, but {ggconsort} provides new, helpful geoms to streamline the process. 

Presenters: Travis Gerke 
Presentation Type: Regular Talk 
Presentation: O24 
Title: CONSORT diagrams in R with {ggconsort} 
 Abstract: CONSORT diagrams are the industry standard graphic for representing participant flow in a clinical trial. Several teams have considered R packages for CONSORT diagram construction, but have fallen short of end-to-end automation. Most notably, Dr. Peter Higgins proposed an excellent CONSORT design overview in his R/Medicine 2020 talk, in which he described the legacy diagram construction as "an artisanal product built by counting categories, then copy and pasting results into templates." Here, I will present a fresh look at the {ggconsort} package, which embraces aspects of CONSORT construction that are inherently artisanal, but eliminates error-prone manual entry. Specifically, I segment CONSORT creation into two stages: (1) CONSORT annotation capture at the time of data wrangling, and (2) diagram layout. I will demonstrate how stage (1) can be built into a single tidyverse chain. Stage (2) maintains some artisanal aspects, but {ggconsort} provides new, helpful geoms to streamline the process. 

Presenters: Taylor Arnold 
Presentation Type: Lightning Talk 
Presentation: O25 
Title: ctrialsgov: Access, Visualization, and Discovery of the ClinicalTrials.gov Database 
 Abstract: In this talk I will present our R package ctrialsgov, which provides functions for accessing and visualizing data from ClinicalTrials.gov’s open access database. The package focuses on providing an easy-to-use interface to clinical trial data along with useful text analysis functions for working with the rich free text response fields present in the dataset. The lightening talk will focus on introduction the package through a case study that investigates how the package could be used to automatically find and sort innovative clinical trial designs for cancer research. The R package is released under an MIT license and currently installable from GitHub. 

Presenters: Emily Zabor 
Presentation Type: Regular Talk 
Presentation: O26 
Title: Designing early phase clinical trials with the {ppseq} package 
 Abstract: This talk will introduce the {ppseq} R package for designing early phase clinical trials using sequential predictive probability monitoring. Clinical trials in oncology increasingly include dose-expansion cohorts to further characterize safety, get preliminary efficacy data, or compare across doses or disease subtypes. But expansion cohorts are often added to trials on the fly, with little planning of the statistical design or consideration for the ethical concerns associated with treating patients at sub-optimal or inefficacious doses. The {ppseq} package provides functionality to design trials using Bayesian sequential predictive probability monitoring. The package includes interactive visualizations that allow users to easily compare designs based on different decision thresholds according to their operating characteristics, and introduces optimization criteria to assist in selecting the ideal design. The functionality of the {ppseq} package will be demonstrated with a re-design of the phase 1 dose-expansion cohort studying the anti-PD-L1 treatment atezolizumab in metastatic urothelial carcinoma. 

Presenters: Jared Huling 
Presentation Type: Regular Talk 
Presentation: O27 
Title: Subgroup identification and precision medicine with the 'personalized' R package 
 Abstract: Heterogeneity of treatment effect is common in medical studies. Improving medical decision making by matching patients with the most effective treatments has the potential to improve treatment efficacy and adherence. Exploratory subgroup analysis allows the identification of clinically relevant subgroups from pre-specified variables for such purpose. In this talk, we will introduce a general framework that encompasses many recent statistical methods for identifying subgroups of patients who may benefit from different available treatments and an R software package, personalized, which implements this general framework. The methods in this framework estimate optimal individualized treatment rules (ITRs) that match patients with treatments by focusing on interactions between the treatments and covariates. We will cover the analysis of data from both randomized clinical trials and observational studies and a wide range of types of outcomes including continuous, binary, count, and times-to-event. This talk will illustrate the usage of this package, from estimation of ITRs for various outcomes to validating and visualizing whether the estimated ITRs result in improved outcomes when applied to new patients. 

Presenters: Irene van Den Broek 
Presentation Type: Lightning Talk 
Presentation: O28 
Title: You R What You Measure: Digital biomarkers for insights in personalized health 
 Abstract: Wearable devices enable continuous, longitudinal collection of physiological or behavioral data. Initially geared towards consumer health enthusiasts, research- and clinical grade wearable devices now find their way into medical research and clinical trials. This talk will highlight the potential of digital biomarkers to advance personalized medicine as well as the central role for R in the connection, integration, analysis, and/or visualization of health data from digital devices.
First, two digital biomarkers with promising clinical utility will be introduced: continuous glucose monitoring (CGM) and heart rate variability (HRV). The discussion will also include personal use experiences and reference to R packages specifically developed for CGM and HRV data analysis. The second part of the talk will showcase examples from a two-year long personal project (you R what you measure) to quantify and visualize health and habits. Use cases include the connection and visualization of data from popular wearable devices and smartphone apps for sleep, activity and productivity tracking, all using the R programming language.
 

Presenters: Steven Schwager 
Presentation Type: Regular Talk 
Presentation: O29 
Title: Graphical Displays in R for Clinical Trials 
 Abstract: Graphical display of clinical trial data can be much more informative than numerical tables and lists. Visualization of study data is an essential tool for evaluating the trial’s progress and evaluating and understanding its outcome. However, creating effective graphics involves art as well as science, requiring careful thought and execution, as is well known. We illustrate a few pitfalls that must be avoided and guidelines for well-designed, powerful graphics, citing the seminal work of Tufte, with focus on clinical trial data. The versatility of R makes it well-suited to creating graphics for exploring the data; monitoring and assessing safety and efficacy; displaying statistical variability; detecting outliers and other anomalies; summarizing the data clearly and correctly; and communicating results to a wide audience, including both regulators and non-statisticians. We present an overview of graphics for clinical trials, including major types of displays, with illustrative examples. We show how R can be used to create innovative graphics by combining approaches and components in novel ways to achieve specialized goals. 

Presenters: Andy South 
Presentation Type: Lightning Talk 
Presentation: O30 
Title: mapping African health data with afrimapr packages, training & community 
 Abstract: The afrimapr project is supporting analysts in Africa to make maps from health data by 1. developing R packages & components 2. providing open-access training materials 3.
initiating a community of users and developers. The R packages can be used to create data visualisations, reproducible reports, and web applications. This includes the ability to make maps from data that are referenced by coordinates or place names. Local data-analysts can be supported to develop or modify their own solutions to
local issues. Data science & R communities are rapidly growing in Africa. R components can be linked to each other and other data systems. Our work eases access to available open data on health facility locations, admin boundaries, sub-national covid case data and population estimates. We conducted the most recent and reproducible review of open access health facility location data for African countries. Demonstration web applications and training materials are available from the afrimapr.org website. In this talk I will demonstrate the range of our packages, training materials and initial community building activities. We welcome contributions. 

Presenters: Julia Silge 
Presentation Type: Regular Talk 
Presentation: O31 
Title: Data visualization for machine learning practitioners 
 Abstract: Visual representations of data inform how machine learning practitioners think, understand, and decide. Before charts are ever used for outward communication about a ML system, they are used by the system designers and operators themselves as a tool to make better modeling choices. Practitioners use visualization, from very familiar statistical graphics to creative and less standard plots, at the points of most important human decisions when other ways to validate those decisions can be difficult. Visualization approaches are used to understand both the data that serves as input for machine learning and the models that practitioners create. In this talk, learn about the process of building a ML model in the real world, how and when practitioners use visualization to make more effective choices, and considerations for ML visualization tooling. 

Presenters: Kristen Panthagani 
Presentation Type: Lightning Talk 
Presentation: O32 
Title: Animated data visualizations with gganimate as a science communication tool during the pandemic 
 Abstract: Unlike any time in recent memory, the challenges, uncertainties, and misinformation surrounding the COVID pandemic have caused the general public to be highly interested in understanding data for themselves. To help address this need, in March 2020 I began creating data visualizations to help the general public understand the growth of the pandemic. Using ggplot2 and gganimate, I create data visualizations that have since been viewed hundreds of thousands of times across multiple social media platforms.  Several features make data gifs particularly effective as science communication tools, including rescaling of axes over time to illustrate exponential growth, creating animated data labels with ggrepel to make graphs very easy to understand, and using beautiful animation as a way to capture attention and increase engagement. In my talk I will briefly highlight how to use these features in R and why they are effective science communication tools. 

Presenters: Emil Hvitfeldt 
Presentation Type: Lightning Talk 
Presentation: O33 
Title: Creating and styling pptx slides with rmarkdown 
 Abstract: {rmarkdown} is a wonderful package that allows us to create many types of outputs. From simple pages to slides, dashboards, and websites. Even though {xaringan} slides have gained a lot of popularity, there is sometimes the need to create slides in Microsoft PowerPoint format. This talk will show you how to create simple .pptx files with {rmarkdown} and how they can be styled to conform with your organization's style. This talk is a formal introduction to the {pptxtemplates} package which contains examples of styled .pptx templates. 

Presenters: Damian Rodziewicz 
Presentation Type: Regular Talk 
Presentation: O34 
Title: R Markdown and {officedown} to Automate Clinical Trial Reporting 
 Abstract: Turn your data to valuable insights and high-quality reports using R Markdown and officedown package to save time spent on manual reporting.  

Presenters: Marcus Adams 
Presentation Type: Regular Talk 
Presentation: O35 
Title: Second Server to the Right and Straight On 'til Production: Deploying a GxP Shiny Application 
 Abstract: In the classic software development text “The Mythical Man-Month” Fred Brooks describes a 9x difference in the effort between creating a program (think a simple app that you run only on your own personal computer) and a programming systems product (or what we may call an app in production). According to a 2019 Burch Works study, however, ~80% of data scientists don’t come from a formal computer science background and therefore likely haven’t read this book. More importantly, though, this also means that they likely do not have experience putting an application or model into production use. They can create wonderous neural networks for splendorous NLP use-cases but lack the experience addressing all the other the requirements which create a robust and dependable product for end users. 

R can and has been put into production by many companies, both large and small. This talk will share insights from the Merck Manufacturing Digital and Data CoE’s experience in launching a GxP reporting Shiny application into production. The speaker, who comes from a chemical engineering background, will share what he learned about the other 89% of what it takes to deploy reliable, secure, and maintainable production applications.
 

Presenters: Will Landau 
Presentation Type: Regular Talk 
Presentation: O36 
Title: Target Markdown and stantargets for Bayesian model validation pipelines 
 Abstract: The {targets} R package enhances the reproducibility, scale, and maintainability of data science projects in computationally intense fields such as machine learning, Bayesian Statistics, and statistical genomics. Recent breakthroughs in the {targets} ecosystem make it easy to create ambitious, domain-specific, reproducible data analysis pipelines. Two highlights include Target Markdown, an R Markdown interface to transparently communicate the entire process of pipeline prototyping and construction, and {stantargets}, a new rOpenSci package that generates specialized workflows for Stan models while reducing the required volume of user-side R code. This presentation demonstrates both capabilities in a simulation-based workflow to validate a Bayesian longitudinal linear model common to clinical trial data analysis.
 

Presenters: John Schwenck 
Presentation Type: Poster Presentation 
Presentation: P11 
Title: bp: Blood Pressure Analysis in R 
 Abstract: Despite the world-wide prevalence of Hypertension, there is a lack of open-source software dedicated to analyzing blood pressure. The R package – bp – fills this void by providing functionality for data processing, visualization, and statistical analysis of blood pressure data. The package implements statistical metrics and visuals from the medical literature on Hypertension and is equipped with six open-source sample datasets covering continuous arterial pressure data, ambulatory blood pressure monitoring (ABPM) data, and home blood pressure monitoring (HBPM) data to help researchers get started. This talk will highlight the main bp package functionality and will illustrate a typical analysis workflow that can be used to generate blood pressure reports.

The bp package can be accessed via CRAN or the development version on GitHub at https://github.com/johnschwenck/bp 

Presenters: Ijeamaka Anyene 
Presentation Type: Poster Presentation 
Presentation: P12 
Title: Tracking Dashboards and Specimen Workflow Management using R and {shinydashboard} 
 Abstract: In the process of creating cohorts for healthcare research, it is often required to consolidate data from various sources. These sources include medical records, lab and pathology results, and data collection software such as REDCap. However, having disparate data sources requires individuals to be skilled in using multiple software systems to 1) have visibility into the data collected and 2) manage any logistics dependent on the ever-changing data. Typically, in research the best way to address this challenge is to use a tracking system. In this talk, I will discuss how I used R and {shinydashboard} to create an internal clinical tracking dashboard. This ecosystem of R software created a centralized location for lead investigators and project managers to see our data collection progress via interactive data visualizations, provided analysts visibility into the characteristics of our cohort, and acted as an operational tool for research staff that allowed them to independently answer data questions and move their own work forward. 

Presenters: Sujata Patil 
Presentation Type: Poster Presentation 
Presentation: P14 
Title: Using free interactive applications to communicate statistical concepts to laboratory researchers 
 Abstract: Statistics literacy is crucial for pre-clinical laboratory researchers engaged in anticancer drug development. We developed a short course in statistics for biomedical researchers using didactic lectures and data examples from published research. Yet, foundational concepts often remain abstract to most researchers. Therefore, we developed computer-based apps that allow biomedical researchers to explore and visualize fundamental ideas at their own pace, thus empowering them to understand and use statistics in their research.

The interactive computer apps covered various concepts, including experimental design, p-values, and multiple comparisons. Our free R Shiny apps facilitate inquiry-led activities to increase motivation and promote statistical thinking and can used by interested colleagues from anywhere in the world, thus democratizing statistics education.

We evaluated the computer apps to assess how well participants were able to comprehend statistical concepts from the beginning to the end of the course and if the apps were useful. We will present our apps as well as results from these evaluations. 
 

Presenters: Deniz Topcu 
Presentation Type: Poster Presentation 
Presentation: P21 
Title: How to get insight about your laboratory? 
 Abstract: A well-organized laboratory has always a key aspect of informed clinical decisions. The modern laboratory produces an unwieldy amount of data. Data analytic tools can be employed to gain insight from otherwise indecipherable amounts of data for decreasing costs, improving process quality, and increasing patient benefit.  Laboratory information systems and middleware can provide insights into the laboratory workflow. However, it is also possible to use R to obtain detailed analytics. In this study developing a web-based analytical tool was aimed at day-to-day usage. Turnaround time, device utilization, staff efficiency, shift workload, test ordering patterns, unnecessary or rarely used tube analysis, and redundant testing analysis can be performed using this tool.  Required data sets can be extracted from LIS or middleware (as a spreadsheet or CSV file) and uploaded into the app. Mandatory and optional fields are provided by template files. Uploaded data first checked for consistency and then the analysis will be performed. Analysis results can be followed as numerical or interactive plots.  Shiny was used to develop a user-friendly interface. ggplot2 and plotly were utilized for interactive plots. 

Presenters: Irina Gaynanova 
Presentation Type: Poster Presentation 
Presentation: P22 
Title: Interpreting blood glucose data with R package iglu 
 Abstract: Continuous Glucose Monitoring (CGM) data play an increasing role in clinical practice as they provide detailed quantification of blood glucose levels during the entire 24-hour period. The R package iglu implements a wide range of CGM-derived metrics for measuring glucose control and glucose variability. The package also allows one to visualize CGM data using time-series and lasagna plots. A distinct advantage of iglu is that it comes with a point-and-click graphical user interface (GUI) which makes the package widely accessible to users regardless of their programming experience. Thus, the open-source and easy to use iglu package will help advance CGM research and CGM data analyses. R package iglu is publicly available on CRAN and at https://github.com/irinagain/iglu. 

Presenters: Sophia Shalhout 
Presentation Type: Poster Presentation 
Presentation: P24 
Title: eLAB: A Large-Scale Laboratory Integration Informatics Pipeline for Clinical Research 
 Abstract: Objective: To develop a clinical informatics pipeline designed to capture large-scale structured electronic health record (EHR) data for a national patient registry. 
Materials and Methods: The EHR-R-REDCap pipeline is implemented using R-statistical software to remap and import structured EHR data into the REDCap-based multi-institutional Merkel Cell Carcinoma (MCC) Patient Registry using an adaptable data dictionary. 
Results: Clinical laboratory data were extracted from EPIC Clarity across several participating institutions. Labs were transformed, remapped and imported into the MCC registry using the EHR labs abstraction (eLAB) pipeline. Forty-nine clinical tests encompassing 482,450 results were imported into the registry for 1,109 enrolled MCC patients. Data-quality assessment revealed highly accurate, valid labs. Univariate modeling was performed for labs at baseline on overall survival (N=176) using this clinical informatics pipeline. 
Conclusion: We demonstrate feasibility of the facile eLAB workflow. EHR data is successfully transformed, and bulk-loaded/imported into a REDCap-based national registry to execute real-world data analysis and interoperability. 
 

Presenters: Serdar Balci 
Presentation Type: Poster Presentation 
Presentation: P31 
Title: Generating reports with R for anatomic pathology laboratory quality control 
 Abstract: Anatomic pathology reports are semi-structured texts, with specific jargon that include sensitive patient information. Laboratory information systems provide statistics and quality control measures but more information is needed from a clinical view. R is a practical way to get more insight from pathology reports.

Istanbul Memorial Healthcare Pathology, serves 8 hospitals in 5 cities. The hospitals use data systems from different vendors and extracted data are available in various formats (csv, json, excel and pdf), but which can be joined via unique patient and biopsy number.

Reports are generated via bookdown. Data are pre-processed in the first chapters, saved as separate RDS files, then read in other chapters as necessary. Bookdown gives flexibility to add new analysis in any place. The reports are rendered with cron jobs.

Various packages and regular expressions are used to label pathology reports, follow up of patients, and generate correlations between cytology-pathology and repeat biopsies. Specimen movements, transfer-reporting time measurements, and laboratory physician workload are calculated. Per disease patient survival analyses are also evaluated. 

Presenters: Jeffrey Nicholas Fisk 
Presentation Type: Poster Presentation 
Presentation: P32 
Title: Calculating Cancer Effect Size to Rank Cancer Drivers Contextually with cancereffectsizeR 
 Abstract: In cancer research, prevalence of particular genetic alterations is often taken as a proxy for importance. However, prevalence and p-values are not themselves measures of effect. As progression of cancer including the acquisition of therapeutic resistance and the mortality-inducing metastatic spread of therapy-resistant cell populations, is fundamentally an evolutionary process, calculation of selection on these variants is an appropriate effect size metric. Here, we present the current version of cancereffectsizeR, an R package that allows for the calculation of the cancer effect size of somatic variants. In addition to calculating the effect from normal somatic tissue to primary progression, cancereffectsizeR also includes the ability to detect stage-specific selection, epistatic interactions, and therapy-induced selection. Overall, cancereffectsizeR provides a quick, easy way to rank-order variants by effect size from tumor sequencing data, empowering guidance of treatment approaches and discovery of resistance mechanisms. 

Presenters: Gergely Daroczi 
Presentation Type: Poster Presentation 
Presentation: P33 
Title: Democratizing Access to Personalized Medicine Using R 
 Abstract: Model-Informed Precision Dosing and PK/PD modeling are still not accessible to the masses -- as gated by expensive software suites and/or complicated interfaces requiring special knowledge. This means that most patients are still treated with potentially suboptimal label doses, while personalized medicine could save not only drug and related costs, but lives as well with better health outcomes.

Rx Studio is an R-based cloud platform providing clinical decision support for precision dosing, using peer-reviewed or custom-built PK/PD/PGx models -- heavily relying on open-source tools, and dedicated to democratizing access to pharmacological models through easy access, free for individuals and education and globally inclusive pricing for clinics and health systems.

This talk provides an overview on the technical platform, the user-facing interfaces and APIs, using R in a cloud infrastructure, difficulties with compliance and international laws when using open-source software, internationalization, and localization of the web interfaces and R packages as well; then discussing opportunities for partnerships with clinical researches, clinical pharmacists and educators. 

Presenters: Miguel Cosenza 
Presentation Type: Poster Presentation 
Presentation: P41 
Title: Proteomics of reverse cardiac remodeling: extracting biological meaning from high-dimensional data 
 Abstract: In the context of cardiac disease, the limited regenerative capacity of the heart can eventually lead to heart failure (HF). Currently, left ventricular assist device (LVAD) implantation is one of the two available therapies. However, in a subset of patients, LVADs promote cardiac unloading and recovery of heart function, allowing LVAD explantation. Characterizing the molecular mechanisms associated with this so-called reverse cardiac remodeling (RCR) is crucial for the identification of predictive biomarkers of cardiac recovery for their use in personalized medicine schemes. Using a mouse model of RCR and mass spectrometry-based proteomics, we were able to identify and quantify thousands of proteins from left ventricular tissue samples. In this talk, I would showcase the use of R for the analysis of this high dimensional data, using (1) visualization approaches (ggplot2) for quality control of the quantitative data, (2) data wrangling methods to explore intrinsic protein degradation processes, and (3) tools for unsupervised (mixOmics) and supervised (limma) analyses to both explore the effect of RCR on protein abundance and identify potential molecular signatures of cardiac recovery. 

Presenters: Piru Perampalam 
Presentation Type: Poster Presentation 
Presentation: P42 
Title: Easy RNA-seq analysis with BEAVR, an R-shiny app 
 Abstract: The use of RNA-sequencing (RNA-seq) in molecular biology research and clinical settings has increased significantly over the past decade. Despite its widespread adoption, there is a lack of simple and interactive tools to analyze and explore RNA-seq data. Many established tools require programming to analyze and visualize results. This requirement presents a significant barrier for many researchers to efficiently analyze and present RNA-seq data.

In this workshop, we will take a look at BEAVR, a Browser-based tool for the Exploration And Visualization of RNA-seq data. Using some publicly available data, we will demonstrate that BEAVR is an easy-to-use tool that facilitates interactive analysis and exploration of RNA-seq data. BEAVR is developed in R and uses DESeq2 as its engine for differential gene expression (DGE) analysis, but assumes users have no prior knowledge of R or DESeq2. BEAVR allows researchers to easily obtain a table of differentially-expressed genes with statistical testing and then visualize the results in a series of graphs, plots and heatmaps. Users are able to customize many parameters for statistical testing, dealing with variance, clustering methods and pathway analysis to generate high quality figures. 

Presenters: Brandon LeBeau 
Presentation Type: Poster Presentation 
Presentation: P51 
Title: Tidy Simulation and Power Analyses 
 Abstract: Power analyses are commonly needed to secure external funding from Federal, State, or local agencies. Many current software implementations for power analyses make assumptions in order for the calculations to be mathematically possible. Unfortunately, the data collected commonly do not meet the assumptions typically made within software used for power analyses. A more flexible and possibly more accurate power analysis framework can be achieved through Monte Carlo simulation. This presentation aims to introduce the benefits and flexibility achieved when conducting a power analysis under a Monte Carlo framework. The presentation will focus specifically on power analyses for general(-ized) linear (mixed) models using an R package called simglm (https://github.com/lebebr01/simglm). This package allows for flexible specification of data simulation conditions that may better approximate real data conditions. In addition, the package allows for the varying of data generating conditions, model fitting conditions, and others to explore impact of specific data characteristics on the empirical power. 

Presenters: Nick Barrowman 
Presentation Type: Poster Presentation 
Presentation: P54 
Title: Exploring subsets in clinical data using the vtree package 
 Abstract: For many scientific data sets, questions about nested subsets arise, but the calculation and visualization of subsets can be time-consuming and error-prone. As the number of nested subsets increases, the magnitude of the task grows rapidly. And if there are missing values in the data set, the task becomes even more complicated. A tree structure provides a natural way to represent nested subsets of a data set. The {vtree} R package is a flexible tool for calculating and drawing "variable trees".

In this workshop, you will learn how vtree can help with a variety of common tasks in clinical research including generating automatic study flowcharts, generating summary statistics for subsets of your data, and examining patterns of missing data. You will also learn about some advanced features of vtree. 

Presenters: Paul Schneider 
Presentation Type: Poster Presentation 
Presentation: P62 
Title: Shiny Decision Modelling 
 Abstract: Statistical models are used ubiquitously across health care to inform decision making. One notable area is health economics, where decision models are a mandatory part of regulatory assessment of the costs and benefits of new treatments.

Traditionally, these models have often been built in MS Excel, but as model complexity increases, R is becoming increasingly popular. However, R lacks a simple point and click user interface. This might make the switch from Excel to R seem daunting, and it makes it difficult to directly communicate model results with decisions makers and other stakeholders.

R Shiny has the potential to resolve this limitation. It allows developers to embed decision models (e.g. economic models, patient decision aids) developed in R into interactive web-interfaces. Users can specify their own preferences and assumptions about model parameters and run different scenario analyses.

In this talk, we provide a brief tutorial on how to wrap a decision model built in R into a Shiny application. As a case study, we use a simple cost-effectiveness model to demonstrate main principles and basic functionality and then explain how this approach can be applied on almost any decision model. 

Presenters: Erika Helgeson 
Presentation Type: Poster Presentation 
Presentation: P63 
Title: Using Shiny to Visualize a Kidney Donor’s Personalized Long-Term Risk 
 Abstract: Individuals considering kidney donation would benefit from understanding their personalized long-term health risks prior to undergoing this life changing medical procedure. Peer reviewed articles may provide cutting edge research about such risks but are often not accessible to the donor candidate nor can the candidate easily determine their personalized risk from these articles. In our presentation, we illustrate how R Shiny can be used to fill this gap: translating scholarly findings into an understandable, user-friendly application.   

We present our work on visualizing long-term risk models for kidney donors. While calculators for donor risk of hypertension, diabetes, proteinuria, and reduced renal function have been published, these calculators are either only presented as model summaries or require familiarity of Excel to generate personalized risk estimates.  To increase accessibility for potential donors and their care team, we adapted these risk models into a user-friendly web-based calculator using Shiny. ,This risk assessment tool provides a comprehensive long-term projection of living kidney donor health in an easy to use and understandable format.  
 

Presenters: Eric Brown 
Presentation Type: Poster Presentation 
Presentation: P64 
Title: A Shiny-based online calculator to estimate the risk of undetected COVID-19 in a congregate setting following an exposure 
 Abstract: High rates of community transmission of COVID-19 lead to possible exposures among patients or residents of congregate settings. The resultant necessary increase in infection prevention and control (IPAC) measures have potential harms such as loneliness and deconditioning. An evidence-based estimation of the risk of the presence of undetected COVID-19 may help to optimize the timing of IPAC measures. We report an innovative Shiny-based online calculator and R package to estimate the probability of an undetected COVID-19 case within a given setting following a potential exposure when there are no symptomatic patients and polymerase chain reaction (PCR) testing is available. The calculator incorporates estimates of incubation period, PCR sensitivity by day of testing, and the estimated fraction of true asymptomatic cases. Our calculator can facilitate evidence-based decisions in a clinical setting or enhance the development of guidelines. The underlying code is publicly available for transparency and accessibility.
 

Presenters: Haocheng Wang 
Presentation Type: Poster Presentation 
Presentation: P71 
Title: Leukemia Analysis & Data Exploration Repository (LeADER) 
 Abstract: Leukemia Analysis & Data Exploration Repository (LeADER) is a data management and visualization platform for cancer clinical trials and correlative laboratory studies at Harvard Medical School. Multidisciplinary research groups face operational inefficiencies and data sharing bottlenecks when performing complex integrative analyses. LeADER bridges the data accessibility gap separating clinicians, bench scientists, bioinformaticians, and statisticians, thereby advancing translational medicine. By linking de-identified clinical, biological, and molecular features of patients, their tumor samples, patient-derived tumor models, and individual tumor cells, collaborators may independently interrogate harmonized, validated, and real-time data.
LeADER comprises a network of linked R Shiny apps, each drawing from a common aggregate data store but deploying unique subsets of data with customized visualization and analysis tools for trial-specific user groups. Distinct features build on existing Shiny functionality to facilitate seamless interaction with complex hierarchical data, such as time series and biospecimen provenance with one to many relationships. Since launch, LeADER has yielded efficiency gains in all steps of the data pipeline. 

Presenters: Haocheng Wang 
Presentation Type: Poster Presentation 
Presentation: P71 
Title: Leukemia Analysis & Data Exploration Repository (LeADER) 
 Abstract: Leukemia Analysis & Data Exploration Repository (LeADER) is a data management and visualization platform for cancer clinical trials and correlative laboratory studies at Harvard Medical School. Multidisciplinary research groups face operational inefficiencies and data sharing bottlenecks when performing complex integrative analyses. LeADER bridges the data accessibility gap separating clinicians, bench scientists, bioinformaticians, and statisticians, thereby advancing translational medicine. By linking de-identified clinical, biological, and molecular features of patients, their tumor samples, patient-derived tumor models, and individual tumor cells, collaborators may independently interrogate harmonized, validated, and real-time data.
LeADER comprises a network of linked R Shiny apps, each drawing from a common aggregate data store but deploying unique subsets of data with customized visualization and analysis tools for trial-specific user groups. Distinct features build on existing Shiny functionality to facilitate seamless interaction with complex hierarchical data, such as time series and biospecimen provenance with one to many relationships. Since launch, LeADER has yielded efficiency gains in all steps of the data pipeline. 

Presenters: Marly Gotti 
Presentation Type: Poster Presentation 
Presentation: P72 
Title: Performing Risk Assessments of R Package Accuracy using Shiny 
 Abstract: In this presentation we introduce the Risk Assessment Shiny application and explain how it can be used to perform a risk assessment of R package accuracy within a validated infrastructure as required within a biopharmaceutical regulatory setting. The Risk Assessment Shiny Application is an interactive web application that serves as an interface to the riskmetric package. Both tools have been developed by the R validation hub, which is a cross-industry initiative funded by the R Consortium. The shiny application portraits the metrics coming from riskmetric, categorized into maintenance, community usage, and testing. The application can be used to record comments on the metrics, which are stored in an underlying database. This makes it possible to stop and start reviews at the reviewer’s convenience. Once a review is complete, a final summary comment can be provided before a final decision is made on the package. In line with the white paper, the decision is an overall risk score: low, medium, or high. The reviewer is then able to generate either an HTML or a DOCX report containing the metrics, comments, and some additional high-level information about the package. 

Presenters: Oriol Senan 
Presentation Type: Poster Presentation 
Presentation: P74 
Title: Fast and Controlled: How to Improve Your Data Analysis Workflow Using Shiny and Pipeline Automation 
 Abstract: Key differences of current data analysis software are the ease and speed at which a user can produce a plot, run a model, or perform an analysis. With this in mind, quality, reproducibility, and the interpretation of results can make the difference between a regular and outstanding analysis. How do you improve quality and ensure reproducibility? Pipeline toolkits are great tools for the control, automation, and management of data analysis workflows. With pipeline toolkits like targets R package, you can automatically run your process, save results and re-run analyses when the outcome is going to change. 
```



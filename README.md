# Capstone Data Science 690 (Draft Proposal)

Proposal By :

Sharath Srinivas

Chetan B Desai

Saideep Malgireddy

# Adverse Reaction of Vaccination : Side Effects Clustering and Risk Prediction methods

![images](https://user-images.githubusercontent.com/60420184/153628674-3a71f712-4f3c-4055-9570-c4a0b5329312.jpg)

### What is your issue of interest (provide sufficient background information)?

There are no vaccine, drug or medical devices which are completely free from the side effects. Vaccine protects many people in Fighting the pandemic like Covid-19. So Its important for any healthcare proffesionals or End users of Vaccine must be aware of the side effects and to prevent any life threathening situtaions.

VAERS: Vaccine Adverse Event Reporting System This method is used to gather information about the type of vaccine administered, the duration of vaccination, the onset of the adverse condition, current diseases or medications, prior history of adverse effects, and demographic information if an individual has an adverse reaction to a vaccine. Any health complications after a vaccine are administered expected by statute to be reported to VAERS by all healthcare providers.
Using VAERS data, on the other hand, must be fully informed of the system's strengths and drawbacks. VAERS data has significant biases. It is impossible to assess the incidence rates and relative risks of various adverse events. Statistical significance tests and confidence intervals should be used with extreme caution to identify the adverse reactions.

### Why is this issue important to you and/or to others?

Anyone who has received a vaccine and had an adverse reaction should file a VAERS report online, even though they are unsure that the vaccine is to blame. So we don't know the overall number of vaccinated people. For Example over 543 million doses of COVID-19 vaccines were administered in the United States from December 14, 2020, through February 3, 2022. During this time, VAERS received 12,122 preliminary reports of death (0.0022%) among people who received a COVID-19 vaccine [1]. It is important to analysis the data during this pandemic and be aware of the information regarding the vaccination.
Anyone can report occurrences to VAERS, even if it is unclear if the problem was caused by a vaccine. As a result, VAERS data cannot be utilized to assess if a reported adverse event was caused by a COVID-19 immunization.# Capstone Data Science 690 (Draft Proposal)

Proposal By :

Sharath Srinivas

Chetan B Desai

Saideep Malgireddy

# Adverse Reaction of Vaccination : Side Effects Clustering and Risk Prediction methods

### What is your issue of interest (provide sufficient background information)?

There are no vaccine, drug or medical devices which are completely free from the side effects. Vaccine protects many people in Fighting the pandemic like Covid-19. So Its important for any healthcare proffesionals or End users of Vaccine must be aware of the side effects and to prevent any life threathening situtaions.

VAERS: Vaccine Adverse Event Reporting System This method is used to gather information about the type of vaccine administered, the duration of vaccination, the onset of the adverse condition, current diseases or medications, prior history of adverse effects, and demographic information if an individual has an adverse reaction to a vaccine. Any health complications after a vaccine are administered expected by statute to be reported to VAERS by all healthcare providers.
Using VAERS data, on the other hand, must be fully informed of the system's strengths and drawbacks. VAERS data has significant biases. It is impossible to assess the incidence rates and relative risks of various adverse events. Statistical significance tests and confidence intervals should be used with extreme caution to identify the adverse reactions.

### Why is this issue important to you and/or to others?

Anyone who has received a vaccine and had an adverse reaction should file a VAERS report online, even though they are unsure that the vaccine is to blame. So we don't know the overall number of vaccinated people. For Example over 543 million doses of COVID-19 vaccines were administered in the United States from December 14, 2020, through February 3, 2022. During this time, VAERS received 12,122 preliminary reports of death (0.0022%) among people who received a COVID-19 vaccine [1]. It is important to analysis the data during this pandemic and be aware of the information regarding the vaccination. Anyone can report occurrences to VAERS, even if it is unclear if the problem was caused by a vaccine. As a result, VAERS data cannot be utilized to assess if a reported adverse event was caused by a Vaccine immunization. So detail analysis required to identify what would have caused the side effects.

### What questions do you have in mind and would like to answer?
1. Can we predict the adverse events associated to vaccine immunization.
2. Cluster Adverse reactions of vaccination in a cluster and gain a thorough understanding of the most common types of adverse reactions, and then to determine whether a person is at a higher risk of suffering a serious adverse reaction that could be life threatening.
3. Predicting the mortality rate of the patient based on the covid vaccination symptoms.
4. Suggesting Vaccination from different manufacturer to the end users based on their Medical History, Allergies and ethicity.
  
### Where do you get the data to analyze and help answer your questions (creditability of source, quality of data, size of data, attributes of data. etc.)?

This project makes use of data from the Vaccine Adverse Event Reporting System (VAERS), which was designed by the Food and Drug Administration (FDA) and the Centers for Disease Control and Prevention (CDC) to receive reports concerning vaccine-related adverse events. Medical practitioners are urged to report adverse events, and VAERS data may include coincidental events that are unrelated to the vaccine.In addition, due to the human factor in data input, we should expect incomplete examples.

<a href="https://vaers.hhs.gov/data/datasets.html">Dataset</a> 

<a href="https://vaers.hhs.gov/docs/VAERSDataUseGuide_November2020.pdf">Data Guide</a>

The VAERS data can be accessed by downloading raw data in comma-separated value (CSV) files.
The following datasets consists of 3 files from year 2010 to 2022: VAERSDATA, VAERSSYMPTOMS, and VAERSVAX. 

VAERSDATA provides the event IDs (VAERS ID) as well as personal information such as age, gender, symptom, allergy type, medical history, deceased, hospitalized, and life threat.

VAERSSYMPTOMS contains The events' IDs and symptom keywords retrieved from the symptom text in VAERSDATA.

VAERSVAX inscribes vaccine types and vaccine manufacturers.

We have select below vaccine as part of our project : 

1. COVID19 (COVID19 VACCINE)
2. EBZR (EBOLA ZAIRE VACCINE)
3. HEP (HEPATITIS B VACCINE)
4. FLU (INFLUENZA)

### What will be your unit of analysis (for example, patient, organization, or country)? Roughly how many units (observations) do you expect to analyze?

Unit of anlysis for our project will be patients, Clinical healthcare Professionals and vaccine manufactures 

### What variables/measures do you plan to use in your analysis (variables should be tied to the questions in #3)?

We will be using adverse reactions, medical history, allergies, gender, age, and vaccine manufacturer.

### What kinds of techniques/models do you plan to use (for example, clustering, NLP, ARIMA, etc.)?

NLP will be used for data cleaning to extract medical history and allergies from the patient information.
We will be using Classification methods such as Random forest, support vector machine, decision tree, K-nearest neighbor and Logistic Regression. Clustring methods like K-Means.

### How do you plan to develop/apply ML and how you evaluate/compare the performance of the models?

A voting classifier and Boosting techniques will be used to determine the accuracy of all the classifiers. We will be using hyper-parameter to tune the model.

### What outcomes do you intend to achieve (better understanding of problems, tools to help solve problems, predictive analytics with practicle applications, etc)?

We plan on providing Web interative application using python Dash for patients and medical professionals which helps them to determine best suitable vacination based on their health records to reduce the life threatening incidents to decide on their vaccine immunization. 

## Reference 
[1]. https://www.cdc.gov/coronavirus/2019-ncov/vaccines/safety/adverse-events.html

[2]. https://pubmed.ncbi.nlm.nih.gov/15071280/


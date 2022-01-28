# OTF_Grants
Automating Ontario Trillium Foundation Grant applications into specific data-informed funding streams
Melissa Hunte (melissar.hunte@mail.utoronto.ca) & Lorena Almaraz De La Garza (l.almaraz@mail.utoronto.ca) 

I.	INTRODUCTION
The Ontario Trillium Foundation (OTF) is one of Canada’s leading granting bodies, with over $730M invested in more than 5K projects helping Ontarians . The OTF has four main grant programs, each of these with unique funding streams—currently, at least ten in total—which determine the kinds of projects and expenses eligible for financial support.
Since 2000, the OTF has approved over 25K applications1. To receive funding, applicants must apply to a specific grant program and funding stream, describing their proposed project. Each year, more than 3K applications are reviewed by hundreds of volunteers1. 
A key responsibility lies in accurately allocating financial resources to suitable applicants. However, the current application process entrusts the program and stream selection to applicants, thereby risking project-stream misalignment. This may increase the likelihood that otherwise eligible programs be denied funding.
II.	BUSINESS OBJECTIVES
As a public agency, ensuring an equitable distribution of funds is a top priority. Yet, the current application and funding processes do not support this aim. Rejecting applications due to a wrongly selected program, for instance, limits access to funds and places undue burdens on applicants. Therefore, creating a streamlined application process might not only remove an unnecessary barrier for users but could increase the likelihood that eligible applications are fairly considered. Further, to ensure funds are meaningfully spent, it is important to certify that funding streams accurately represent applicants’ needs. With this in mind, we propose two objectives:
1)	To create a system that sorts general applications into exisiting grant programs. With neatly defined criteria for each program, we propose a classifying algorithm to sort general applications into existing programs. The model, using project descriptions, would allow for applications to be effortlessly sorted internally, simplifying the process for applicants and volunteer reviewers, reducing error.
2)	To define funding streams that accurately reflect applicants’ needs. We propose a clustering technique to identify and define applicants’ expenditure priorities, informed by almost 28K successful applications. Since it is unclear how current funding streams were determined, in the interest of transparency and efficiency, we recommend a data-driven. This will ensure funding streams are representative of the needs of applicants.
3)	III.	RESULTS
A.	Classify general applications into exisiting programs.
Using the project descriptions, our machine learning model can predict with reliable accuracy (95%) which program grant an application is best suited for. The selected model was a Random Forest classifier, which outperformed an initial Multinomial Naïve Bayes model. Due to the sporadic nature of programs, as shown in Figure 1, it is recommended to adjust the model as programs arise or shift in future.
 
Fig. 1.	A scatterplot shows inconsistency in grant programs across time.
B.	Cluster project descriptions to create funding streams.
Our clustering model determined nine unique funding streams, created from almost 28K project descriptions from successful applications. These clusters tell us that over the last 20 years, applicants have consistently mentioned these priorities in their applications. Figure 2 shows the clusters and top five associated keywords.
 
Fig 2. Clusters capture unique interests as noted in project descriptions.
Based on these findings, we recommend nine new, data-informed fundings streams: 1. Equipment Upgrade Fund, 2. Accessibility Improvement Fund, 3. Community Impact Fund, 4. Organization Capacity-Building Fund, 5. Safety Improvement Fund, 6. Heritage and Culture Fund, 7. Volunteer Support & Training Fund, 8. Programme Development Fund, 9. Youth & Child Programme Fund.


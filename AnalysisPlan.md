#Analysis Plan

#Summary 

What I am interested in is performing a double mediation analysis on my current dataset as well as visualization of the mediation model. My key variables of interests are: 1. Subjective Social Class (IV), 2. Personal Relative Deprivation (M1), 3. Social Dominance Orientation (M2) and 4. Lay Belief about Social Class (DV). The structure of my study is a survey done through Qualtrics. In the study, I plan on removing for participants that complete the study in too short of an amount of time. On each page of my survey, there is a timer. Participants that complete the page in less time than the number of items/questions on each page multiplied by 1.5 seconds will be removed from the analysis. M1, M2 and our DV are previously validated scales and compose of several items/questions. We will be creating three composite measures for M1, M2 and DV using the items associated with each of those scales. 

I will be conducting the analysis in R Studios and I will be using the following packages (to my current knowledge): psych, tidyverse, car, laavan, semPlot, dtplyr, and dplyr. 

#Pseudocode 

#Set Workspace
Import psych, tidyverse, car, laavan, semPlot, dtplyr, and dplyr packages 
Set working directory to import dataset 
Import dataset 

#Clean Data for Analysis
Remove participants that did not provide consent to our study
Remove participants that did not provide us consent to use their data (via the debrief form)
Filter results of page 1 to remove any participants that complete the page faster than the number of items on that page x1.5 seconds
	Repeat for all 6 pages in the study (excluding the consent and the debrief forms) 
	
#Create Composite Variables
Average the items for M1 to create the first composite measure
	Repeat for M2 and DV to create all three composite measures needed for the study

#Analysis
Create the model for double mediation analysis using laavan syntax
Take the model created and summarize result as well as create the sem plot 

	


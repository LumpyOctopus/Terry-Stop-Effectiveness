# Phase 3 Project:  Terry Stops
#### The data set that I chose was from the Seattle Open Data website (https://data.seattle.gov/Public-Safety/Terry-Stops/28ny-9ts8).  The purpose of this project is to determine the effectiveness of the Terry stop, as well as to predict whether or not a stop resulted in arrest.  
###### The definitions for each column are as follows:

Subject ID: Key, generated daily, identifying unique subjects in the dataset using a character to character match of first name and last name. "Null" values indicate an "anonymous" or "unidentified" subject. Subjects of a Terry Stop are not required to present identification.

GO/SC Num: General Offense or Street Check number, relating the Terry Stop to the parent report. This field may have a one to many relationship in the data.

Terry Stop ID: Key identifying unique Terry Stop reports.

Stop Resolution: Resolution of the stop as reported by the officer.

Weapon Type: Type of weapon, if any, identified during a search or frisk of the subject. Indicates "None" if no weapons was found.

Officer ID: Key identifying unique officers in the dataset.

Officer YOB: Year of birth, as reported by the officer.

Officer Gender: Gender of the officer, as reported by the officer.

Officer Race: Race of the officer, as reported by the officer.

Subject Perceived Race: Perceived race of the subject, as reported by the officer.

Subject Perceived Gender: Perceived gender of the subject, as reported by the officer.

Reported Date: Date the report was filed in the Records Management System (RMS). Not necessarily the date the stop occurred but generally within 1 day.

Reported Time: Time the stop was reported in the Records Management System (RMS). Not the time the stop occurred but generally within 10 hours.

Initial Call Type: Initial classification of the call as assigned by 911.

Final Call Type: Final classification of the call as assigned by the primary officer closing the event.

Call Type: How the call was received by the communication center.

Officer Squad: Functional squad assignment (not budget) of the officer as reported by the Data Analytics Platform (DAP).

Arrest Flag: Indicator of whether a "physical arrest" was made, of the subject, during the Terry Stop. Does not necessarily reflect a report of an arrest in the Records Management System (RMS).

Frisk Flag: Indicator of whether a "frisk" was conducted, by the officer, of the subject, during the Terry Stop.

Precinct: Precinct of the address associated with the underlying Computer Aided Dispatch (CAD) event. Not necessarily where the Terry Stop occurred.

Sector: Sector of the address associated with the underlying Computer Aided Dispatch (CAD) event. Not necessarily where the Terry Stop occurred.

Beat: Beat of the address associated with the underlying Computer Aided Dispatch (CAD) event. Not necessarily where the Terry Stop occurred.

##### It is important to note that the "Arrest Flag" does not necessarily mean that the arrest was made at the time of the stop.
###### In analyzing the data, we are able to break the data down and make correlations.
![arrests](https://user-images.githubusercontent.com/96254640/197403880-b1ece363-24aa-4c6d-9742-12384d3f8987.png)

###### Here we can see that approximately 25% of stops end in arrest.  However, in the next graph, we see that approximately only 9% of the stops result in arrests at the scene.
![arrestsduringandafter](https://user-images.githubusercontent.com/96254640/197403923-bd784179-35a7-4285-888b-74eb8c252720.png)

###### When making models, I selected KNN, Logistic Regression, Decision Tree, and Random Forest Classifiers.  Though all of the models were close in prediction, the Random Forest model was the most accurate, giving roughly an 85% prediction rate.
### Conclusion
###### The study shows us that while approximately 25% of the stops result in arrest, only 9% end up in arrest during the stop.  This shows us that it is not an effective means of arresting criminals.  If the use of these stops are to get guns off the street, they are not an effective tool either, as less than 5% of those stops that resulted in arrest yielded firearms.  This study also illuminates a need for police training.  Police should be trained in filling out paperwork completely.  While the model can predict to an approximate 85% accuracy arrest rate, the model could predict more accurately the arrest rate if all of the blanks are filled in.  Furthermore, given the low arrest rates, police should be trained on when to enact a Terry stop.
### For More Information
##### For a full analysis see [Jupyter Notebook](https://github.com/LumpyOctopus/Phase3_Project/blob/main/Phase%203%20Project.ipynb) or review the presentation [here](https://github.com/LumpyOctopus/Phase3_Project/blob/main/Presentation.pdf).
Data gathered from [Seattle Open Data website](https://data.seattle.gov/Public-Safety/Terry-Stops/28ny-9ts8).

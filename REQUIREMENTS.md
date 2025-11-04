Requirements Elicitation Lead:

1- Requirement Elicitation Techniques Used:

1- Surveys:
Purpose: Collecting peoples Experience with Checking a Car’s History.

Questions asked:
1- Have you ever bought or sold a used car?
2- How did you check the car’s history?
3- How confident are you that the information sellers provide about a car is accurate?
4- What problems have you faced when trying to verify a car’s history?

Outcomes:
1- The majority have bought a car with a minority selling them.
2- Some have asked the seller directly and taken it to mechanic with the others only doing one of the two.
3- The majoirty tend to distrust the sellers honesty when it comes to the information about the car.
4- People found it hard to get accurate information with most finding inaccurate and unclear information about the car, missing records, sometimes even false ones.

2- Stakeholder Interviews:
Purpose: To understand the expectations and needs of potential system users.

Participants: 
1- Car buyer 
2- Car seller

Questions asked:
1-	What are the challenges that you experience when checking a car’s background?
2-	What kind of car information would make you trust the system?
3-	What makes you doubt the accuracy of current car check systems?
4-	How useful would a price estimation feature be?

Outcomes:
1-	Buyers want quick, clear, and trustworthy car records.
2- Resellers value transparency to build customer trust.
3-	Both groups emphasized the need for reliable data.
4-	Both groups appreciated the idea of AI price estimation.

2- Team Brainstorming Process Documentation:

Agenda:
1- Define project purpose and scope.
2- List all user expectations and technical needs.
3- Group ideas into requirement categories.
4- Discussing feasibility and prioritizing requirements.

Collected Ideas:
1-	VIN & plate number lookup.
2-	Display car’s past damages and unpaid fines.
3-	Secure, fast, and accurate data retrieval.
4-	Regular updates for reliability.
5-	Simple, clear, and user-friendly design.
6-	Predict approximate car value using AI.

3- Raw requirements list: 

The system shall allow users to input VIN and plate number.

The system shall display all the car's records (accidents, fines, repairs).

The system shall receive all records from the traffic police database to ensure data accuracy.

The system shall allow the owner of the car to add additional records verified via receipts.

The system shall ensure data security.

The system shall estimate the car’s current market value using AI.

The interface shall be simple and user-friendly.


2- Requirements Classification Specialist:

The requirements will be classified in this order:
1- The requirement
2- Type of functionality
3- Type of Requirement

Requirement Table:

1- The system shall allow users to input VIN and plate number/ Functional/ User Requirement

2- The system shall display all of the car's records/ Functional/ User Requirement

3- The system shall receive all records from the traffic police database to ensure data accuracy/ Functional/ System Requirement

4- The system shall allow the owner of the car to add additional records verified via receipts/ Functional/ User Requirement

5- The system shall ensure data security/ Non-Functional/ System Requirement

6- The system shall estimate the car’s current market value using AI/ Functional/ User Requirement

7- The interface shall be simple and user-friendly/ Non-Functional/ System Requirement


3- Structured Specification List


| function      | Receive User Input: Vehicle Identification Number (VIN) and plate number.|
| ------------- | ---------------------------------------------------------------------------------------------------------------- |
| Description   | Receives the input values (ex: VIN/Plate number) that a user enters into the systems UI.                                                                                                                                                                                       |
| Inputs        | Vehicle Identification Number (VIN) and plate number.                                                                                                                                                                                                                          |
| Source        | User Input Form.                                                                                                                                                                                                                                                               |
| Outputs       | Search query gets sent to the backend                                                                                                                                                                                                                                          |
| Action        | The user will have a page and in that page it will contain a form where they can enter a VIN or Plate number so that they can search for a specific car they would like to see displayed and                         during that, the system will take the search query and process it in the backend. |
| Requires      | A form for the user to input their values into.                                                                                                                                                                                                                                |
| Precondition  | Link or a page that has the Input form.                                                                                                                                                                                                                                        |
| Postcondition | Search terms get stored for later in listing vehicles.                                                                                                                                                                                                                         |


| function      | Display all available car records.                                                                                                                              |
| ------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Description   | Displays all available car records such as accidents, fines and repairs through the UI.                                                                         |
| Inputs        | System database and traffic police API.                                                                                                                         |
| Source        | System database and traffic police API.                                                                                                                         |
| Output        | Displays each car record in a container on the UI.                                                                                                              |
| Action        | The system will display all available cars within the database including their accidents fines and repairs on a page if the user has left the search box empty. |
| Requires      | A UI to display the car records to a user.                                                                                                                      |
| Precondition  | Search query is empty.                                                                                                                                          |
| Postcondition | Displays each car record in a container on the UI.                                                                                                              |
| Side Effects  | No Cars Available or API goes down.                                                                                                                             |


| function      | Estimation of a car’s current market value using AI.                                                                                                                                                                                                   |
| ------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Description   | The system will use an AI agent to estimate the price of a car that is selected by taking into account the data relating to it, like accidents, repairs and fines                                                                                      |
| Inputs        | Selected Car, List of fines/Accidents.                                                                                                                                                                                                                 |
| Source        | Selected car from database and car history from the traffic police API.                                                                                                                                                                                |
| Output        | Response from the AI agent displaying the data within the UI.                                                                                                                                                                                          |
| Action        | The AI LLM will take the information relating to a vehicle selected by the user and based on its own data or predefined values within our own app, it will make an estimation of the price of the                    car and then display it next to the car on the page. |
| Requires      | LLM and A selected car                                                                                                                                                                                                                                 |
| Precondition  | Page of a selected car.                                                                                                                                                                                                                                |
| Postcondition | Estimated value of selected car displayed next to it.                                                                                                                                                                                                  |
| Side Effects  | Nonsensical values being estimated by the LLM or the LLM API is down.                                                                                                                                                                                  |


5- Prioritized requirements list

| Requirement                                                                                   | Priority | Reason                                                                                                           |
| --------------------------------------------------------------------------------------------- | -------- | ----------------------------------------------------------------------------------------------------- |
| The system shall allow users to enter a Vehicle Identification Number (VIN) and plate number. | M        | This is a core aspect of our app since it allows users to start the search of the specific car record                                                                                                                 they want. |
| The system shall display all available car records such as accidents, fines, and repairs.     | M        | This is an important part of our app so that users can actually see all the history for a car they                                                                                                                    searched for.                                                                                        |
| The system shall receive all records from the traffic police API to ensure data accuracy.     | M        | This is where most of the car data comes from.                                                        |
| The System shall ensure data security.                                                        | M        | This is vital since we are dealing with sensitive user data such as VIN/plate numbers.                |
| The system shall estimate the car’s current market value using AI.                            | N        | This would be very useful but isn't vital to the systems initial core functionality                   |
| The interface shall be simple, intuitive, and easy to navigate.                               | N        | This would be nice to have but it can also have a basic UI.                                           |



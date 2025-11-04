CAR INSPECTOR USE CASE DOCUMENTATION 

EXTERNAL USERS OR SYSTEMS;

• USER (Owner, buyer); 
− Can create account for using app 
− Can log in to account if there exists 
− Allowed to show cars history  
− Allowed to show cars specifications 
− Allowed to enter car’s information 
− Allowed to only check fines and not allowed to modify it 
− Allowed to show the car’s trusted estimated price provided by app  
− Users can give feedback for app to have better experience 

• POLICE STATION; 
−  Can add vehicle information (Registration details, Plate number, VIN number) 
−  Can add the accident reports of car’s 
−  Can add or delete fines 

• SYSTEM ADMINISTRATION; 
− System admin can manage users 
− Can keep application updated to keep application from performance lose and 
security concerns 
− Can review system feed backs to optimize and fix system issues 
− Can check the pricing mechanism 
 
• MECHANICS / AUTHORIZED DEALERSHIP SERVICES; 
− Services can create an authorized account 
− Services can log in to authorized account if there exists 
− Services can add maintenance or fixing records they have done to the car 
 
• ARTIFICAL INTELLIGANCE 
− AI can check and store car’s specifications with history to search within app 
and online sources to provide estimated market value for cars to provide to 
the user.        

Internal Systems
                                  
Log in; System will check if the account that user tries to login exists or not. If it exists user 
will log in but if it doesn't exist user will get an error message  
 
Display cars estimated price: If user opens this tab, the system will automatically connect 
to a subsystem controlled by AI. This subsystem will check the owner's car’s information, 
history and then it will find the car’s that has certain specifications to that car 
Validation; Validation depends on the registration details that the police station has. This 
connection system can validate the entered plate number and Vin number of car. 
Car history; User, police station and mechanics can add records or display the history of 
car after validation of the plate number and VIN number of car.  
Check fines: Checking fines by user is connected to fines segment in system to prevent any 
type of changes by user. Fines are controlled by police station, and they can add new fines 
or delete the paid ones from system.


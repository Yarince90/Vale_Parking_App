# ValetParkingApp
Final Project for OOP244 at Seneca College (CPA Program)
==========================================================
Overview: 
This program manages a "Valet Parking" that can store a dynamically allocated number of vehicles,
the vehicles can be either a "car" with the option of having the carwashed or not 
and a "motorcycle" with the option of the motorcycle having a sidecar or not.
The tester Main module for this program does copy from a backup file to the one being used 
before the program ends within the "ShowDataFile()" function.

Details:
This program promts up a Menu with the following 5 options:
1- Park vehicle
2- Return Vehicle
3- List Parked Vehicles
4- Close Parkinf (End of day)
5- Exit program

1-) The first option (Park vehicle) will prompt up a sub-menu with the following options: 
    1- Car 
    2- Motorcycle 
    3- cancel.
if option 3 is selected (cancel) the user will be re-directed to the main menu with the 5 options again.
if either option 1- Car or 2- Motorcycle is selected the program will create a new object of either one and prompt
the user to enter a Licence Plate Number, a Make and Model and to enter either "Y" or "N" to wash car while parked (if it's a car)
or to enter "Y" or "N" if if has a side car (if it's a motorcycle).

Once the information has been properly filled out, the program will generate a "Parking Ticket" displaying the information entered as well as the Parking Spot Number
NOTE: the Licence Plate will be turned to upper case.

2-) The second option (return vehicle) will allow the user to enter a Licence of a parked vehicle in order to "return" the vehicle to the owner
NOTE: caps do not matter when searching for License plate as it will internally turn it to uppercase
if a match is found the program will delete the vehicle object and assign nullptr to the parking spot where that vehicle was located and return to user to the main menu
along with a message that containing "Returning" + the details for that vehicle and updating the number of parking spots availible.

3-) The third option just goes through the array of the parked vehicles and lists them as this:
Vehicle type:
Parking Spot Number:
Licence Plate:
Make and Model
With Carwash/Sidecar or blank

4-) Second last option number 4 closes the parking for the day it propmpts an "Are you sure?" message which accepts either a "y" for yes or a "n" for no if an "n" is entered it aborts it and goes back to the main menu, otherwise it "towes" all the vehicles in the parking lot which deletes all vehicles in the array plus the array.

5-) lastly option number 5 will also prompt an "Are you sure?" message which accepts either a "y" for yes or a "n" for no if an "n" is entered it aborts it and goes back to the main menu otherwise it exits the program.
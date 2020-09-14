# Garbage_Truck_Monitoring_System

To run the project, first clone the repo or download the zip and execute the following command which will install the required packages
> pip3 install -r requirements.txt

Then, to run the Django project, simply execute
> python manage.py runsever

Garbage Truck Monitoring System is a role based system having three roles admin, driver and a citizen. Admin has a dashboard from which admin can add resources such as drivers, bins, depot, dumping ground and vehicles. Admin will have facility of viewing the current data in the system and monitor the drivers in real time. 

![Alt text](screenshots/dashboard.jpeg?raw=true "Dashboard")


The new bin location can be added by just clicking on the map or writing the address of the actual location. Its capacity and height needs to be entered as those parameters will be used to calculate real time garbage level of the bin.  

![Alt text](screenshots/addBin.jpeg?raw=true "Add a bin")


The bin status will be shown to admin wherein bins are classified into three categories based on the level of garbage. Red, yellow and green bins represent overfilled bin, normally filled bin and underfilled bin respectively.

![Alt text](screenshots/binStatus.jpeg?raw=true "Bin Status")


The routes will be generated using our algorithm which follows the approach followed by CVRP algorithm. Daily, routes will be generated taking into account the real time garbage level, capacity of vehicles, the distance between bins, etc. G Maps API provides an efficient way and real time distances according to the traffic parameter for the inputs.  

![Alt text](screenshots/routes.jpeg?raw=true "Routes")

The visualization of CVRP is given as follows.

![Alt text](screenshots/CVRP.jpeg?raw=true "CVRP")

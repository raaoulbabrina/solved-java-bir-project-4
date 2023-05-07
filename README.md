Download Link: https://assignmentchef.com/product/solved-java-bir-project-4
<br>
In this assignment, you will apply the following concepts you learned in java (abstract class, interfaces,Polymorphism,exception handling,Files manipulation and encapsulation) .

<strong><u>Palestinian Vehicle Agency: </u></strong>A vehicle of three types (car, minivan, and truck) has many attributes.

<strong>[Question] Designing Vehicle class and Its Sub-classes There are several Vehicles for transportation such as Car, MiniVan, and Truck. Details of the classes for the vehicles are shown in the Figure1</strong>

<strong><u>Request of the question:</u></strong>

<strong>Write Java program code to realize the Figure .1</strong>

<strong>Description of the fields and methods of the classes as follows:</strong>

<ol>

 <li><strong>For Fields</strong>

  <ul>

   <li><em>Model-name: </em>Model name of a vehicle</li>

   <li><em>Brand: </em>Company to produce the model</li>

   <li><em>Owner: </em>Owner of the vehicle (as object)</li>

   <li><em>Engine-type: </em>Type of the engine. Classified by fuel type to be used such as gasoline, diesel, or hybrid  <em>Tank-size: </em>Size of fuel tank. Unit is liter.</li>

   <li><em>Fuel-consumption: </em>Fuel consumption. Unit is km/liter.</li>

   <li><em>numberOfSeats: </em>Integer number of seats in a vehicle.</li>

   <li><em>airConditionOn: </em>Boolean status of air-condition’s working: ON/OFF.</li>

   <li><em>hasAutoDoor: </em>Boolean status of a vehicle’s having auto door.</li>

   <li>power: Horse Power of a vehicle’s engine.</li>

   <li>Diesel is public static final int=1, and gasoline is public static final int =2</li>

  </ul></li>

 <li><strong>For Methods</strong>

  <ul>

   <li><strong><em>Movable-distance(): </em></strong>Getting information of movable distance of a vehicle when the tank of the vehicle is filled fully.</li>

   <li><strong><em>costFor100Km(Petroleum-Price): </em></strong>Calculating cost for running 100Kms with the engine type and the petroleum type passed by as parameter. It will be different according to fuel and air-condition’s status.</li>

   <li><strong><em>setAirConditionON</em></strong>: Setting the air-condition of the vehicle to ON.</li>

   <li><strong><em><u>You can guess other methods.</u></em></strong></li>

   <li><strong><em>You have to add your owns methods, at <u>least one additional </u>method for each class, other than mentioned above.</em></strong></li>

   <li>Create appropriate setters and <strong><em>getters for classes.</em></strong></li>

  </ul></li>

 <li><strong>Some conditions to write methods</strong>

  <ul>

   <li>The Car uses only gasoline engine.</li>

   <li>The Minivan can use engine of both gasoline and diesel. But the fuel consumption is same for both gasoline and diesel.  The Truck uses only diesel engine.</li>

   <li>The engine type Hybrid uses only gasoline.</li>

   <li>Default air-condition status is OFF, and the air-condition can be ON/OFF after instances being created by <em>setAirConON/setAirConOFF </em></li>

   <li>Default fuel consumption is considered when air-condition is OFF.</li>

   <li>Fuel consumption of the Car increased by 10% when air-condition of the Car is ON.</li>

   <li>Fuel consumption of the Minivan and the Truck increased by 20% when air-condition of the Car is ON.</li>

   <li>For Petroleum Price: Gasoline(get price from console NIS/liter , for instance 5.23 NIS/liter)), Diesel(get price from console NIS/liter, for instance 4.02 NIS/liter)</li>

   <li>Use <strong><u>Exception Handling </u></strong>to handle errors caused by mismatch filling type of Petroleum , throw an <u>illegal argument exception</u></li>

   <li>Date: you have to use Calender class (Gregorian calender).</li>

   <li>Use <em>StringBuilder class </em>to deal with string manipulations when read from file. ( splitting,</li>

  </ul></li>

</ol>

uppercase,lowercase,….etc)

Appropriately implement the above hierarchy and stick to the following

All Vehicle objects are comparable based on the <strong><u>costFor100Km . </u>Clone an instance of </strong>Vehicle object, without cloning the

owner of this Vehicle (<em>set the owner to null for cloned object</em>) Using deep cloning. toString() method should be implemented in appropriate way in all Vehicle sub classes displaying all the information including the <em>costFor100Km</em>.

Create a <strong><u>menu </u></strong>that allow user to select from them as the following:

<ol>

 <li>Read the data about objects from the file <em>“inputdata.txt” </em>and store them in</li>

 <li><em>Set prices of petroleum.</em></li>

 <li>Print sorted order Vehicles in an ascending order based on costFor100Km.</li>

 <li>(<strong><em><u>Bonus </u></em></strong>) Print sorted order Vehicles in an ascending order based on <em>owner name </em>.</li>

 <li>(<strong><em><u>Bonus </u></em></strong>) Print sorted order Vehicles in an descending order based on vehicle brand.</li>

 <li>Clone Vehicle without owner. (Ask user to choice one object for cloning from Arraylist, after Listing them to user ) 7. Turn air-condition on</li>

 <li>Write Output on the “<em>txt</em>” file after sort them.</li>

 <li>Exit from System</li>

</ol>

<strong><u>Note: </u></strong>when turn air-condition is on, you can again select one of steps 3-6, the output should be print on file.

<strong><u>The file input format is:</u></strong>

Car,Camley,E100,Toyota,Ahmad,Gasoline,70.0,15.15,5

Car,Aqua,ES500,Toyota,Nader,Hybrid, 36.0, 40.0, 5

MiniVan,Sienna,A4,Toyota,Malik, Gasoline,75.0,9.0,8,true

MiniVan,Odyssey,S500,Honda,Khaled, Diesel, 56.0,11.0, 8,false

MiniVan,Presage,BX5000,Nissan,Shaher, Gasoline,60.0,7.0,7,false

Truck,Tundra,EDGE500,Toyota,Sami,Diesel,100.,6.76,5,310

Truck,Ridgeline,DUG700,Honda,Waleed,Diesel,83.279,7.23,5,250

Sample of printed line on out file:

ModelName: Camley, Brand: Toyota, Owner: Ahmad, EngineType: Gasoline, TankSize: 70.0,

FuelConsumption: 15.15, NumberOfSeat: 5, Movable distance: 1060.5 Km, Cost for 100 Km: 46.90 NIS
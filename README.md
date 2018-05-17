# vehicleInheritanceSuperExample
A question on the quiz got me fucked up. Apparently, simply using super(privateInstanceVarFromSuperClass) allows us to access the superclass private instance variables. WTF?

Look at the constructors for subclass LandVehicle and Auto. Instead of utilizing a setType method(which doesn't exist in the superclass), they simply write: 

    super(type) = parameterVariable;
    
and now LandVehicle, for example, has its type instance variable. Here is an example not in the stock main program.

  LandVehicle myLandVehicle = new LandVehicle("ATV");
  System.out.println("MyLandVehicle type = " + myLandVehicle.displayInfo());
  
  which is the same for both the direct subclass of vehicle, LandVehicle, AND FOR IT's subclass, Auto.



  

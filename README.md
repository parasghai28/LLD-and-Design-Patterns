# LLD-and-Design-Patterns

DESIGN PRINCIPLES
_________________

Methods defined in a class represents the behaviour that instances of that class will have during runtime.
Associations deifne a relationship between classes. There are multiple types of association - 

Dependeny Association - 

public class Vehicle{
  public void break() {
    Syso("break");
  }
  
   public void run() {
    Syso("run");
  }
}

public class Driver{
  public void drive(Vehicle car)  { //Driver recieves Vehicle object only in scope of drive(), Driver is dependent on Vehicle to perform drive()
    car.run();
  }
}


Composition Association- A particular object is composed of other objects. Composition implies ownership. If the containing object ceases to exist, then
internal objects which are part of it ceases to exist. 

public class Vehicle{

  Tyre tyre; //Vehicle has composition association with Tyre, if vehicle ceases to exist so does Tyre;
  public vehicle(Tyre aTyreObj) {
    tyre = aTyreObj;
  }
}


Aggregation Association - It does not apply ownership unlike composition. It is less restricted form of Composition where entities can remain alive even
if one ceases to exist

public class HistoryCourse {
  Student[] registeredStudents;
}

FORMING ASSOCIATIONS B/W OBECTS
_______________________________

When thinking about forming association b/w objects, do not only think about how objects behaviour, but also about your application behaviour 

SOFTWARE DESIGNS (SOLID princilples)
_______________

SINGLE Responsibilty Principles(S) - A class should only know about one thing 




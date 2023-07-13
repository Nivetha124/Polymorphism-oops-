# Polymorphism-oops-

POLYMORPHISM
 *   Implementing same method(FUNCTION) in different context(CLASS)
 *   Methods with same name implementing in different way.
  
# Real time example:
   *   we have three classes: "CAR", "BOAT", and "PLANE", and they all have a method called "MOVE()"
   *   You act as a STUDENT when you are at college, you act like a SON/DAUGHTER when you're at home, you act like a FRIEND when you're surrounded by your friends.
   *   a man at the same time is a father, a husband, an employee. So the same person posses different behavior in different situations.
   *   A mobile phone we can use as a CALL,a SEARCHING SOMETHING, a SAVE OUR PHOTOS.
     eg:
class Car:
  def __init__(self, brand, model):
    self.brand = brand
    self.model = model

  def move(self):
    print("Drive!")

class Boat:
  def __init__(self, brand, model):
    self.brand = brand
    self.model = model

  def move(self):
    print("Sail!")

class Plane:
  def __init__(self, brand, model):
    self.brand = brand
    self.model = model

  def move(self):
    print("Fly!")

car1 = Car("Ford", "Mustang")       #Create a Car class
boat1 = Boat("Ibiza", "Touring 20") #Create a Boat class
plane1 = Plane("Boeing", "747")     #Create a Plane class

for x in (car1, boat1, plane1):
  x.move()


# Inheritance Class Polymorphism
class Vehicle:
  def __init__(self, brand, model):
    self.brand = brand
    self.model = model

  def move(self):
    print("Move!")

class Car(Vehicle):
  pass

class Boat(Vehicle):
  def move(self):
    print("Sail!")

class Plane(Vehicle):
  def move(self):
    print("Fly!")

car1 = Car("Ford", "Mustang") #Create a Car object
boat1 = Boat("Ibiza", "Touring 20") #Create a Boat object
plane1 = Plane("Boeing", "747") #Create a Plane object

for x in (car1, boat1, plane1):
  print(x.brand)
  print(x.model)
  x.move()



# Design-Patterns
Easy explanation of different design patterns






**Factory Deisgn Pattern**: Creating Object of a class in another class rather in main class() showing to the user
We want to hide the implementation/real class call from the user side. Suppose user will give input to create what type of ice cream they want but there will be no direct object creation of that class. Another interface will get that type and call the real class to creat object.

strawberry _icecream implements ice_creame{              
Void taste()
{
output(“strawberry”);

}

}


Mango_icecream  implements ice_creame{

Void taste()
{
output(“Mango”);

}
}


Chocolate_icecream  implements ice_creame{

Void taste()
{
output(“Chocolate”);

}


}

Interface Icecream{

Void taste();

}


Class icecream_factory{

Ice_cream get_intance(string flavour)
       if(flavour==’mango’)
{
Return new Mango_icecream();
}
Else if(){
}
Else{

}



}




Class User{

Public stattic void main (String [] args)
{

Icecream_factory obj= new icecream_factory();
Ice-cream s=obj.get_instance(“mango”);
s.taste();




}



}









**Builder Design Pattern**
(creating class + initialization) in a interface

Summary: If we want to create Object of a class with a constructor parameter means an interface will get all the info  from the setter and then it will return the main object.



**Adapter Design Pattern**
(Making a class equals to another with the help of a interface )
When two interfaces are incompatible and their legacy cannot be change we define another adapter class that make them equal. It means one class will implement same interface as 1st class and will take the 2nd class obj to store its data to pretend to be 2nd class. Its like mimic with his costume
Now thats equal
Why adapter design pattern is simpler to understand without charger analogy | LLD | Low Level Design





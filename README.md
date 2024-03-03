# overriding-run-time-polymorphism
import java.util.*;
class Animal {
  void print()
  {
    System.out.println("parent class");
  }
}
class Dog extends Animal {
  void print()
  {
    System.out.println("Dog barks");
  }
}
class Cat extends Animal {
  void print()
  {
    System.out.println("Cat meows");
  }
}
class Main {
  public static void main(String[] args)  {
  Animal a;
  a = new Dog();
  a.print();
  
  a = new Cat();
  a.print();
  }
}


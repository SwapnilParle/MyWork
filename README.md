# MyWork
About Training

# 1. Abstract Example
package Assignments;

abstract class Animal {
     public abstract void animalSound();
    // Regular method
    public void m1() {
        System.out.println("regular method");
    }
}

class Pig extends Animal {
    public void animalSound() {
        System.out.println("The pig says: wee wee");
    }
}

class Main {
    public static void main(String[] args) {
        Pig myPig = new Pig(); // Create a Pig object
        myPig.animalSound();
        myPig.m1();
    }
}


# 2. Anonymous Example
package First_Code;

interface a{
    void show();
}
public class AnonymousFunction {
    public static void main(String[] args) {


        a A = new a() {
            @Override
            public void show() {
                System.out.println("we are creating anonymous function");
            }
            // we implemented function here so we dont need to create a class
        };
        A.show();
    }
}
// we cannot create a object of interface so for that we need to create another class to implement the methods
// of interface.


# 3. Inheritance simple example
package Assignments;
class A{
    public void show(){
        System.out.println("this is class a");
    }
}
class B extends A{
    public void show(int a){
        System.out.println("integer"+ a);
    }
}
public class inheritance extends B{
    public static void main(String[] args) {
        A ojb = new A();
        B obj1 = new B();
        obj1.show();
        obj1.show(5);
    }
}


# 4. Interface
package Assignments;
interface AB{
    void M1();
}
interface BC{
    void M2();
}
public class InterfaceExample implements AB, BC {
    @Override
        public void M1 () {
            System.out.println("from method M1 of interface AB");
        }

        @Override
        public void M2 () {
            System.out.println("from method M1 of interface AB");
        }

    public static void main(String[] args) {
        InterfaceExample obj2 = new InterfaceExample();
        obj2.M1();
        obj2.M2();
    }
    }


# 5.  Encapsulation
package Assignments;

class Student {
	// private data member
	private String name;

	public String getName() { // getter method for name
		return name;
	}

	public void setName(String name) { // setter method for name
		this.name = name;
	}
}

public class Encapsulation {
	public static void main(String[] args) {
//creating instance of the encapsulated class  
		Student s = new Student();
//setting value in the name member  
		s.setName("Swapnil");
//getting value of the name member  
		System.out.println(s.getName());
	}
}













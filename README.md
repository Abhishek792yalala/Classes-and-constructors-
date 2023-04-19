# Classes-and-constructors-
class Outer{

    Outer(){

        System.out.println("Outer class constructor");

    }

    {

        System.out.println("Outer class instance block");

    }

    class Inner{

        Inner(){

            System.out.println("Inner class constructor");

        }

        {

            System.out.println("Inner class instance block");

        }

    }

    public static void main(String... args){

        new Outer().new Inner();

    }

}

/*

Outer class instance block

Outer class constructor

Inner class instance block

Inner class constructor

 */

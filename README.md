# Basic-Java-Information
Information for Beginning Java
# METHODS 
Methods in Java present a way to structure code better. It allows the developer to write once and use multiple times. Methods run only when called inside of the program.

### Basic Structure 
public static void methodName(){
    System.out.println("Testing");
}

The above method, called methodName creates a new line that prints out "Testing" when run.
To run the method, use methodName(); elsewhere in the program

Example:
***
    public static void main(String[] args) {
        methodName();

    }

    public static void methodName() { //Void means **do not send any data back, no return**
        System.out.println("Testing");
    }

***
### Passing Data Into a Method
Methods in Java allow you to take data into a method without initilizing it elsewhere in the code. Adding variable types and names into the () of the method will take data in that can then be manipulated.
Example:
***
    public static void main(String[] args) {
        methodName(1, 30); // Tells the method how many hours and minutes are going to be used in the calculation

    }

    public static void methodName(int hours, int minutes) { // Defines what variables are going to be used in the method
       int seconds = (((hours * 60) * 60) + (minutes * 60)); // Converts hours to minutes, to seconds, and adds the minutes to seconds conversion
        System.out.println("There are " + seconds + " in " + hours + " and " + minutes + " minutes."); // Prints out the result
    }
***
Important Information:
**void** instructs the method not to return any data, this is useful for printing 
**to return data**: return is used to return data to the main class, doing this requires the method to be structured as follows:
public static int methodName() // This states that the method is returning an integer value


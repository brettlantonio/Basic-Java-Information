<h1>Switch Statements</h1>
A switch statement is a cleaner way to write an "if-else" code block. It can be used with Ints, Chars, Shorts, Bytes, and Strings (**note when using strings, set the string to all lower or upper case as the switch is case sensitive**) . It is comprised as follows:

 int switchValue = 1;

        switch(switchValue) {
            case 1:
                System.out.println("Value was one");
                break;
            case 2:
                System.out.println("Value was two");
                break;
            default:
                System.out.println("Was not 1 or 2");
In the above statement, a variable "switchValue" is initialized and the switch method is started using the switch(switchValue) statement.
Each "if-else" statement is written as "Case x" which translates to "if switchValue = x". A break statement terminates the code if that switch value is met.
The "else" statement takes the term "default" meaning "If none of the above are true, default to this statement.

It is possible to combine code statements to make code segments shorter as follows:
int switchValue = 1;

        switch(switchValue) {
            case 1:
                System.out.println("Value was one");
                break;
            case 2:
                System.out.println("Value was two");
                break;
            case 3: case 4: case 5:
                System.out.println("Value was three, or 4, or 5");
                System.out.println("Actually it was a " + switchValue);
                break;
            default:
                System.out.println("Was not 1 or 2");


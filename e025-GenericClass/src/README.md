- When we define a new class, we must know the type of data with which we will work.
- If we want to perform a specific operation within this new class, whatever the type of data it will receive, we can make use of the generic types.
- This generic type will assume the type of data that we will actually pass on to the class.
- Example:
    ```
    // Class Generic
    public class Generic<T>
    {
        private T obj;
    
        public Generic(T o)
        {
            obj = o;
        }
    
        public void classType()
        {
            System.out.println("The type of T is: " + obj.getClass().getName());
        }
    }
    ```

    ```
    // Class Main
    public class Main
    {
        // Methods
        void init()
        {
            Generic<Integer> iObj = new Generic<Integer>(10);
            iObj.classType();

            Generic<String> sObj = new Generic<String>("Hello world");
            sObj.classType();
        }

        // Main method
        public static void main (String args[])
        {
            new Main().init();
        }
    }
    ```

    ```
    output:
        The type of T is: java.lang.Integer
        The type of T is: java.lang.String
    ```

- T is the generic type that will be replaced by a real type. (it only works with objects).
- Conventions for generics:
    - T: Type (represents a type)
    - K: Key (for maps)
    - N: Number (for numbers)
    - E: Element (for Java Collections Framework)
    - V: Value (represents the value)
    - S,U,V: (represents other types)

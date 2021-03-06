- Swing is a library of graphical user interfaces (GUI) for Java.
- It comes included with the Java development environment (JDK).
- Extends to another older graphic library called AWT.

- The JFrame class provides operations to manipulate windows.
- After creating the object you have to:
    - Set the size
    - Set the closing action.
    - Make it visible.


- Example:
    ```
    import javax.swing.*;
    public class Main
    {
        public static void main (String args[])
        {
            JFrame f = new JFrame("Title");
            f.setSize(600, 600);
            f.setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);
            f.setVisible(true);
        }
    }
    ```

- Closing actions:
    - JFrame.EXIT_ON_CLOSE: Quit application.
    - JFrame.DISPOSE_ON_CLOSE: Releases the resources associated with the window.
    - JFrame.DO_NOTHING_ON_CLOSE: It does not do anything.
    - JFrame.HIDE_ON_CLOSE: Close the window, without releasing its resources.

- The normal thing is to create a class, extend JFrame, and perform the initialization operations in its constructor or in an init method.

# Layouts

- The layouts define the distribution that the components will have.
- Every container must have a layout assigned.
- Initially everyone has a defined one, in case we want to work with that.
    - The JFrame has a BorderLayout assigned.
    - And the JPanel a FlowLayout.


### BorderLayout

- The BorderLayout locates the elements in five different zones, north, south, east, west and center.
- Instance:
    ```
    BorderLayout borderLayout = new BorderLayout();
    BorderLayout borderLayout = new BorderLayout(x, y);   // Separation between components
    ```
- Add items:
    ```
    getContentPane().setLayout(borderLayout);
    getContentPane().add(element1, BorderLayout.CENTER);
    getContentPane().add(element2, BorderLayout.NORTH);
    getContentPane().add(element3, BorderLayout.SOUTH);
    getContentPane().add(element4, BorderLayout.EAST);
    getContentPane().add(element5, BorderLayout.WEST);
    ```


### FlowLayout 

- The FlowLayout places the elements horizontally or vertically.
- Place the elements in a row by dividing the space between them and if there is not enough space, jump to the next row.
- Instance:
    ```
    FlowLayout flowLayout = new FlowLayout(FlowLayout.CENTER, 5, 5);    // Alignment and separation between components
    ```

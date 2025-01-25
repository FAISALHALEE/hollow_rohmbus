# Hollow Rhombus Pattern Generator

## Overview
This program generates a **hollow rhombus pattern** using Java. It takes an integer input `n` that specifies the size (number of rows) of the rhombus and prints the corresponding hollow rhombus pattern on the console.

---

## Code Explanation

### 1. **Package and Imports**
The program uses the `java.util.*` package, although it is not explicitly needed in this implementation.

### 2. **hollow_rohmbus Method**
This is the core method that generates and prints the hollow rhombus pattern.

#### Steps:
1. **Outer Loop (`i`):**
   - Controls the rows of the rhombus (1 to `n`).
2. **First Inner Loop (`j`):**
   - Adds leading spaces to shift the stars and create the rhombus shape.
3. **Second Inner Loop (`j`):**
   - Prints `*` for the boundary (first or last row, or first/last column).
   - Prints spaces (` `) for the hollow part inside the rhombus.
4. **New Line:**
   - After completing each row, a new line is added using `System.out.println()`.

### 3. **Main Method**
The `main` method calls the `hollow_rohmbus` method with a fixed size `6`. This size can be adjusted or replaced with user input to make the program dynamic.

---

## Sample Output
For `n = 6`, the program produces the following output:
```
     ******
    *    *
   *    *
  *    *
 *    *
******
```

### How It Works:
1. The first line is fully filled with stars (`*`).
2. Subsequent lines have a star (`*`) at the start and end of the row, with spaces (` `) in between.
3. The final line is fully filled with stars, completing the hollow rhombus.

---

## Usage
1. Compile and run the program using:
   ```bash
   javac hollow_rohmbus.java
   java hollow_rohmbus
   ```
2. You can modify the input size in the `main` method to generate different rhombus sizes.

---

## Customization
- To accept user input for `n` dynamically, use the `Scanner` class:
  ```java
  Scanner sc = new Scanner(System.in);
  System.out.print("Enter the size of the hollow rhombus: ");
  int n = sc.nextInt();
  hollow_rohmbus(n);
  ```
- Replace the hardcoded value `6` in the `main` method with the variable `n`.

---

## Notes
1. Ensure the input `n` is a positive integer greater than or equal to 1.
2. This code currently uses spaces to align the rhombus shape; it assumes a monospaced font for proper formatting.

---

## Example for `n = 4`
Input:
```
4
```
Output:
```
   ****
  *  *
 *  *
****
```

---

## Author
This program was written as a simple Java exercise to demonstrate nested loops and pattern generation.

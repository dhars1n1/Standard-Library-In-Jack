# Standard-Library-jack

# Jack Standard Library

## Introduction

This initiative aims to enhance the Jack programming language by providing a robust set of data structures and utility functions. Jack, being a low-level object-oriented language, lacks a comprehensive standard library found in more mature languages like Java or Python. Our custom standard library addresses this gap, enabling developers to write more efficient and effective code.

## Features

This library includes the following features:

### Data Structures
- List: A dynamic array that can grow or shrink in size.
- Vector: A resizable array providing efficient index-based access.
- Queue: A first-in-first-out (FIFO) data structure.
- Priority Queue (pQueue): A queue where each element has a priority, and higher priority elements are dequeued first.
- Matrix: A two-dimensional array supporting matrix operations.
- Binary Search Tree (BST): A tree structure that maintains elements in sorted order.
- Hash Table: A data structure that maps keys to values for efficient lookups.
- Set: A collection of unique elements.

### Utility Functions

#### Sorting Algorithms
- Bubble Sort: A simple sorting algorithm that repeatedly steps through the list, compares adjacent elements, and swaps them if they are in the wrong order.
- Insertion Sort: A sorting algorithm that builds the final sorted array one item at a time.
- Selection Sort: A sorting algorithm that repeatedly selects the smallest (or largest) remaining item and moves it to the correct position.
- Quick Sort: A highly efficient sorting algorithm that uses a divide-and-conquer approach

#### String Manipulation
- String Comparison: Compares two strings lexicographically.
- toUppercase: Converts all characters in a string to uppercase.
- toLowercase: Converts all characters in a string to lowercase.
- String Reversal: Reverses the characters in a string.

#### Mathematical Operations
- Greatest Common Divisor (GCD): Computes the largest number that divides two integers without leaving a remainder.
- Exponentiation: Raises a number to the power of an exponent.
- Finding the Hypotenuse of a Triangle: Calculates the hypotenuse of a right-angled triangle using the Pythagorean theorem.
- Cube Root Calculation: Computes the cube root of a number.

## Getting Started

### Prerequisites

To use the Jack Standard Library, you need:
- The Jack compiler and virtual machine (VM).
- Basic understanding of the Jack programming language.


### Execution

# Step-by-Step Instructions for Executing Jack Code and Running the Obtained VM Code

## Prerequisites

1. **Jack Compiler and VM Emulator**: Ensure you have the Jack compiler and VM emulator installed. These are typically provided as part of the NAND2Tetris software suite.
2. **Jack Code**: Make sure you have your Jack code files ready.

## Step 1: Writing Jack Code

Create your Jack code file(s) with a `.jack` extension. For example, you might have a file named `Main.jack`.

## Step 2: Compiling Jack Code to VM Code

1. **Open the Jack Compiler**: Open the Jack compiler. This can be done using the command line or the graphical interface provided by NAND2Tetris.
   

2. **Select the Directory**: Choose the directory where your `.jack` files are located. The compiler will process all `.jack` files in the selected directory.



3. **Compile the Code**: Start the compilation process. The compiler will convert the Jack code into VM code, generating `.vm` files.

### Command Line Compilation

If you are using the command line, navigate to the directory containing your Jack files and run:

```sh
JackCompiler Main.jack
```


This will generate a `Main.vm` file in the same directory.

   
## Step 3: Running the VM Code in the VM Emulator

1. **Open the VM Emulator**: Open the VM emulator provided by NAND2Tetris.



2. **Load the VM Code**: In the VM emulator, load the `.vm` file(s) generated by the compiler.

   - Click on the "Load Program" button.
   - Navigate to the directory containing the `.vm` files.
   - Select the appropriate `.vm` file(s). For example, select `BubbleSort.vm` and `Main.vm`.



3. **Configure the VM Emulator**: Ensure the VM emulator is set up correctly. You may need to configure the memory, CPU, and other settings based on your program requirements.

 

4. **Run the VM Code**: Start the execution of the VM code.

   - You can step through the code line by line using the "Step" button.
  


   - Use the "Run" button to execute the code continuously.
  


### VM Emulator Controls

- **Step**: Executes one VM instruction at a time.
- **Run**: Continuously runs the VM code until it completes or is manually paused.
- **Pause**: Pauses the execution of the VM code.
- **Reset**: Resets the VM emulator to its initial state.

### Example Execution

1. Load the `BubbleSort.vm` and `Main.vm` file.
2. Configure any necessary initial settings.
3. Click "Run" to execute the program.
4. Observe the output and debug as needed.

## Step 4: Debugging and Testing

- Use the VM emulator’s debugging tools to inspect the state of the stack, memory, and registers.
- Verify the program's output and behavior.
- Adjust and recompile your Jack code as necessary to achieve the desired results.

    
   
By following these steps, you can effectively compile and run all the Jack programs, leveraging the custom standard library to enhance the programming capabilities in the Jack environment.

### Installation

1. Clone the repository to your local machine:
    ```sh
    git clone https://github.com/your-repository/jack-standard-library.git
    ```

2. Navigate to the project directory:
    ```sh
    cd jack-standard-library
    ```

3. Compile the Jack files using the Jack compiler.

### Usage

After compiling the Jack files, you can include the necessary modules in your Jack programs. Here are examples of how to use some of the provided features:

#### Example: Using the List Data Structure

```jack
class Main {
    function void main() {
        var List myList;
        let myList = List.new();
        do myList.add(5);
        do myList.add(10);
        do myList.remove(0);
        let myList.get(0);
        return;
    }
}
```

#### Example: Using the Bubble Sort Function

```jack
class Main {
    function void main() {
        var Array myArray;
        var int size;
        let size = 5;
        let myArray = Array.new(size);
        let myArray[0] = 5;
        let myArray[1] = 3;
        let myArray[2] = 8;
        let myArray[3] = 4;
        let myArray[4] = 2;
        do Sort.bubbleSort(myArray, size);
        return;
    }
}
```

### Documentation

Detailed documentation for each data structure and utility function is available in the `docs` directory. It includes descriptions, method signatures, and usage examples.

## Contributing

We welcome contributions to the Jack Standard Library! If you have a feature request, find a bug, or want to add a new data structure or utility function, please open an issue or submit a pull request.

### How to Contribute

1. Fork the repository.
2. Create a new branch:
    ```sh
    git checkout -b feature/YourFeature
    ```
3. Make your changes.
4. Commit your changes:
    ```sh
    git commit -m 'Add some feature'
    ```
5. Push to the branch:
    ```sh
    git push origin feature/YourFeature
    ```
6. Open a pull request.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

We would like to thank the Jack programming language community for their support and contributions. Your feedback and collaboration are invaluable in making this project a success.

---

By building and utilizing this standard library, we aim to significantly expand the capabilities of the Jack programming language, providing developers with essential tools for efficient programming. We hope this project serves as a valuable resource for the Jack community. Happy coding!

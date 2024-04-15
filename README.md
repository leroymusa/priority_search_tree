# Priority Search Tree

## What is a Priority Search Tree?

A Priority Search Tree (PST) is a data structure used for efficient searching in multidimensional space, particularly in computational geometry. It is an extension of binary search trees designed to handle multidimensional data.

## How does it work?

A Priority Search Tree organizes points in a balanced binary tree structure, where each node represents a range along one dimension. This allows for efficient range queries and point insertion and deletion operations.

## What does the project do?

The PrioritySearchTree.java project implements a Priority Search Tree (PST) in Java. It provides functionality to construct a PST from a set of points and visualize the resulting tree structure. The implementation includes methods for building the PST using bottom-up heap construction, performing heapify operations, and printing the tree for visualization purposes.

## Usage

To use the PrioritySearchTree.java implementation, follow these steps:

1. Compile the PrioritySearchTree.java file.
2. Create an array of points (external nodes) to represent the input data.
3. Initialize a PrioritySearchTree object with the array of points.
4. Call the `buildPrioritySearchTree()` method to construct the PST.
5. Call the `printTree()` method to visualize the resulting tree structure.

## Example

```java
public class Main {
    public static void main(String[] args) {
        Point[] points = { 
            new Point("p1", -8, 3), new Point("p2", -7, 1), 
            new Point("p3", -1, 6), new Point("p4", 2, 4),
            new Point("p5", 4, 8), new Point("p6", 5, 9), 
            new Point("p7", 7, 1), new Point("p8", 9, 7) 
        };

        PrioritySearchTree.testPrioritySearchTree("Example", points);
    }
}

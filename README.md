# HTMLTreeJava

**HTMLTreeJava** is a Java application that demonstrates tree data structures using Java Swing. It constructs a sample HTML-like tree containing elements such as `html`, `head`, `body`, `meta`, `title`, `ul`, `li`, `h1`, `h2`, and `a`.

The application displays the hierarchy in a graphical tree view and prints information about the tree structure and traversal orders in the console.

## Features

- Builds a hierarchical tree using `DefaultMutableTreeNode`.
- Displays the tree using Swing's `JTree`.
- Identifies the root node.
- Demonstrates parent and sibling relationships.
- Displays child nodes and one-level subtrees.
- Prints each node's level in the hierarchy.
- Calculates and displays tree depth.
- Displays the degree, or number of children, of each non-leaf node.
- Demonstrates breadth-first, preorder, and postorder traversal.

## Requirements

- Java Development Kit (JDK) 21
- A Java-compatible IDE, such as NetBeans, or a terminal
- A graphical desktop environment to display the Swing window

## Project Structure

```text
HTMLTreeJava/
├── pom.xml
├── README.md
└── src/
    └── main/
        └── java/
            └── com/
                └── mycompany/
                    └── htmltree/
                        └── HtmlTree.java
```

## How to Run

### Option 1: Using NetBeans

1. Clone or download the repository.
2. Open the project in NetBeans as a Maven project.
3. Ensure JDK 21 is configured.
4. Run the `HtmlTree` main class.
5. View the tree in the Swing window and inspect the console output.

### Option 2: Using Maven

Clone the repository:

```bash
git clone https://github.com/ichiroyamazaki/HTMLTreeJava.git
cd HTMLTreeJava
```

Compile the project:

```bash
mvn compile
```

Run the application:

```bash
mvn exec:java
```

The Maven configuration specifies `com.mycompany.htmltree.HtmlTree` as the main class.

## Tree Structure

The application constructs a hierarchy similar to the following:

```text
html
├── head
│   ├── meta
│   └── title
└── body
    ├── ul
    │   ├── li
    │   └── li
    ├── h1
    └── h2
        └── a
```

This is a sample tree made from HTML element names. The program does not parse an actual HTML document.

## Tree Traversal Methods

The application uses Java's built-in tree enumeration methods:

- **Breadth-first traversal:** Visits nodes level by level.
- **Preorder traversal:** Visits a node before its descendants.
- **Postorder traversal:** Visits descendants before their parent.

It also uses custom methods to print node levels, sibling groups, child relationships, tree depth, and node degrees.

## Concepts Demonstrated

- **Tree data structures:** Represents hierarchical relationships between nodes.
- **Java Swing:** Uses `JTree` and `JFrame` to display the tree.
- **`DefaultMutableTreeNode`:** Creates nodes that can contain child nodes.
- **Recursion:** Traverses the hierarchy to examine node relationships.
- **Tree enumeration:** Demonstrates different traversal orders.
- **Maven:** Defines the project build configuration.

## Limitations

- The tree structure is predefined in the source code.
- The application does not load or parse external HTML files.
- The interface displays the tree but does not provide a full HTML editor.
- The program is intended as a learning example rather than a production HTML parser.

## Author

**Ichiro Yamazaki**

## License

No license is specified in the repository. Check the repository for licensing information before redistributing or modifying the project.

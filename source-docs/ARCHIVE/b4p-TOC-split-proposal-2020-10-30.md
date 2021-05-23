b4p-TOC.md

-----------------------------------------------------------------------------
==> THIS SHOULD GO INTO THE TABLES SECTION OF THE FUNCTION LIBRARY,
OR CREATE A SEPARATE 'TABLE FUNCTIONS'  GUIDE AND PUT ALL TABLE-RELATED
FUNCTIONS THERE. 


    4 Tables
        4.1 Accessing Tables
            4.1.1 Simple Table Access
            4.1.2 Horizontal Table Access
                4.1.2.1 Horizontal Table Access w. Param. Sets
                4.1.2.2 Horizontal Table Access w. Wildcards
                4.1.2.3 Horizontal Table Access w. Ranges
            4.1.3 Vertical Table Access
                4.1.3.1 Vertical Table Access w. Param. Sets
                4.1.3.2 Vertical Table Access w. Wildcards
                4.1.3.3 Vertical Table Access w. Ranges
            4.1.4 Matrix Table Access
            4.1.5 Partial Table Specification
            4.1.6 Nested Partial Table Specification
            4.1.7 Shifted Table Column Specifications
            4.1.8 Header Name Exception Handling
            4.1.9 Lookup Access Exception Handling
        4.2 Header Names - Memory Effect



-----------------------------------------------------------------------------
USER GUIDE

```text
1 Overview
    1.1 What is B4P?
    1.2 Benefits and Features
    1.3 Use Cases
    1.4 B4P Concepts

2 Installation and Setup
    2.1 Windows
        * Prerequisites
        * Intallation
        * Post-installation optimization
    2.2 MacOS
        * Prerequisites
        * Intallation
        * Post-installation optimization
    2.3 Linux
        * Prerequisites
        * Intallation
        * Post-installation optimization

3 Starting B4p
    3.1 Interactive Mode
    3.2 Programming Mode

4  Help
    4.1 Interactive Mode Help
    4.2 Web documentation
    4.3 PDF documentation

5 Tutorials
    5.1 Introduction to Programming in B4P
    + 5.2 B4P Program Examples



```

-----------------------------------------------------------------------------
TECHNICAL GUIDE

    1 Licensing

    2 Standards and Conventions
        2.1 UNICODE Character Set
            2.1.1 Case Sensitivity
            2.1.2 HTML Entities
            2.1.3 Console Input / Output
            2.1.4 Loading and Saving Files
            2.1.5 CSV File Format
        2.2 Basic Data Types
            2.2.1 Literals
                2.2.1.1 Literals - Indexing
                2.2.1.2 Literals - Extracting Substrings
            2.2.2 Numerals
            2.2.3 Dates
            2.2.4 Booleans
            2.2.5 Voids
            2.2.6 Parameter sets
                2.2.6.1 Parameter sets - Indexing
                2.2.6.2 Parameter sets - Extracting Subsets
                2.2.6.3 Parameter sets - Value Ranges
                2.2.6.4 Parameter sets - Value Repetitions
        2.3 Reserved keywords
        2.4 Path and File Names
        2.5 Locales
        2.6 Comments
    3 Variables
        3.1 Variable Scopes
            3.1.1 Global Variables
            3.1.2 Local Variables
            3.1.3 System Variables
                3.1.3.1 List of System Variables
        3.2 Variable Attributes
        3.3 Variable Forms and Trees
            3.3.1 Simple Variables
            3.3.2 Arrays
            3.3.3 Structures
            3.3.4 Zero Members Variables
            3.3.5 Parameter Sets Specifying Members
        3.4 References to Variables
            3.4.1 Simple References
            3.4.2 Through-Referencing
            3.4.3 Redirecting References
            3.4.4 Copying References
            3.4.5 Releasing References
            3.4.6 References in Member Variables
        3.5 Protecting Variables

    5 Formulas and Operators
        5.1 Unary Operators
        5.2 Binary Operators
            5.2.1 Arithmetic Operators
                5.2.1.1 Additions
                5.2.1.2 Subtractions
                5.2.1.3 Multiplications
                5.2.1.4 Divisions
            5.2.2 Comparison Operators
                5.2.2.1 Equal to
                5.2.2.2 Not Equal to
                5.2.2.3 Strictly Equal to
                5.2.2.4 Strictly Not Equal to
                5.2.2.5 Smaller than (or Equal to)
                5.2.2.6 Greater than (or Equal to)
            5.2.3 Comparison Options
                5.2.3.1 Wildcards
                5.2.3.2 Logical Operators
                5.2.3.3 Logical And
                5.2.3.4 Logical Or
        5.3 Deep Operators
            5.3.1 Deep Unary Operators
            5.3.2 Deep Binary Operators
            5.3.3 Matrix Operations Summary
        5.4 Assignment operators
        5.5 Deep Assignment Operators
        5.6 Ad-hoc Operators
            5.6.1 Cascading ad-hoc Operators
            5.6.2 Ad-hoc Operators Overview
    6 Transactions
        6.1 Without Transaction Assignment Operators
            6.1.1 Transactions between Variables
            6.1.2 Transactions from Tables to Variables
            6.1.3 Transactions from Variables to Tables
            6.1.4 Transactions between Tables
        6.2 & Transaction Assignment Operators
            6.2.1 & Transactions between Variables
            6.2.2 & Transactions from Tables to Variables
            6.2.3 & Transactions from Variables to Tables
            6.2.4 & Transactions between Tables
        6.3 | Transaction Assignment Operators
            6.3.1 | Transactions between Variables
            6.3.2 | Transactions from Tables to Variables
            6.3.3 | Transactions from Variables to Tables
            6.3.4 | Transactions between Tables
        6.4 + Transaction Assignment Operators
            6.4.1 + Transactions between Variables
            6.4.2 + Transactions from Tables to Variables
            6.4.3 + Transactions from Variables to Tables
            6.4.4 + Transactions between Tables
    7 Functions and Procedures
        7.1 Function Parameters
        7.2 Function Parameter Directions
        7.3 Function Parameter Types
            7.3.1 Parameter Set or Literal (Func. Param. Type)
            7.3.2 Table Columns (Func. Param. Type)
            7.3.3 Code Pieces (Func. Param. Type)
                7.3.3.1 Comparison Expressions (func. params)
                7.3.3.2 Expressions (func. params)
                7.3.3.3 Variables (func. params)
                7.3.3.4 Statements (func. params)
            7.3.4 Expressions to Select Rows
        7.4 Indirect Parameter Passing



-----------------------------------------------------------------------------
FUNCTION LIBRARY

    8.1 Control Flow Functions
        + 8.1.1 Loops
        + 8.1.2 Branches
        + 8.1.3 User-Defined Procedures and Functions
        + 8.1.4 Start or include Beyond4P Programs
        + 8.1.5 Exception Functions
        + 8.1.6 Comparison and Selection Functions
        + 8.1.7 Code Execution Functions
        + 8.1.8 Other Control Flow Functions
    8.2 Input / Output Functions
        + 8.2.1 Text Input / Output
        + 8.2.2 Console Special Effects
        + 8.2.3 Inspection and Debugging
    8.3 Type Conversion and Formatting Functions
        + 8.3.1 literal, quoted literal, softquoted literal
        8.3.2 numeral
        8.3.3 clean (if) numeral
        8.3.4 smart (if) numeral
        8.3.5 date, pure date, date time
        8.3.6 time, pure time
        8.3.7 Date and Time Detection Rules
        8.3.8 boolean
        8.3.9 parameter set
        8.3.10 join ...
        8.3.11 type, type detailed
        8.3.12 hash signature
        8.3.13 excel column number
    8.4 Mathematics and Statistics
        + 8.4.1 Basic Math Functions
        + 8.4.2 Transcendental Functions
        + 8.4.3 Series Functions
        + 8.4.4 Matrix Functions
        + 8.4.5 Statistics Functions
        8.4.6 Conditional Combination Functions
        + 8.4.7 Finance and Business Functions
    8.5 String Functions
        + 8.5.1 String Search and Extraction Functions
        + 8.5.2 Character Encoding and Decoding
        + 8.5.3 Miscellaneous String Functions
    8.6 Date and Time Functions
        + 8.6.1 Date Functions
        + 8.6.2 Time and Stopwatch Functions
        + 8.6.3 Sleep and Wait Functions
    8.7 Parameter Set Functions
        + 8.7.1 Set Search and Extraction Functions
        + 8.7.2 Matrix Manipulation Functions
    .8 Table Functions
        + 8.8.1 Creating and Deleting Tables
        + 8.8.2 Accessing Table Information
        + 8.8.3 Accessing Table Contents
        + 8.8.4 Loading and Saving Tables
        + 8.8.5 Input/Output with Tables
        + 8.8.6 Checking and Processing Headers
        + 8.8.7 Searching Tables
        + 8.8.8 Processing Table Columns
        + 8.8.9 Processing Table Rows
        + 8.8.10 Processing Table Contents
        + 8.8.11 Renaming, Copying and Splitting Tables
        + 8.8.12 Checking and Comparing Tables
        + 8.8.13 Looking up Other Tables
        + 8.8.14 Pivoting and Conosolidating Tables
        + 8.8.15 Combining Multiple Tables
        + 8.8.16 Exploring and Extracting Tables
    8.9 Formatting and Styling Tables
        + 8.9.1 Defining User Specific Colors
        + 8.9.2 Styling Functions
        + 8.9.3 Finishing up formatting
    8.10 Variables Functions
        + 8.10.1 Basic Variables Functions
        + 8.10.2 Arrays and Structures
        + 8.10.3 Loading and Saving Variables
        + 8.10.4 Variable References Functions
        + 8.10.5 Resident Attributes Functions
    8.11 Directory and File System Functions
        + 8.11.1 Basic Directory and File Functions
        + 8.11.2 Listing and Searching Directories and Files
        + 8.11.3 Manipulating Directories and Files
        + 8.11.4 File Compression and Decompression
    8.12 System Functions
        + 8.12.1 Executing System Commands
        8.12.2 set locale
        8.12.3 Registry Access Functions
        + 8.12.4 Licensing and Privileges
    8.13 Help and Support Functions
        8.13.1 help
        8.13.2 docs
        8.13.3 web docs
        8.13.4 view
        8.13.5 view reset
        8.13.6 list / explain functions
        8.13.7 dump functions
    8.14 Cross-Functional Info
        8.14.1 Sorting and Ranking Options
        8.14.2 Consolidation Actions

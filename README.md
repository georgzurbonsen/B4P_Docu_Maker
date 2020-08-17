# B4P_Docu_Maker
Utility to create B4P documents


## Required files:
  **Build_Docu.b4p** compiles all raw text material and generates all HTML files in the subdirectory "Output".
  Attention: You need to specify the right path to the C source file in order to capture all what you have.  See top of file
  
  **Inputs** contains *enhanced* JSON files with contents not related to specific function names.  All function specific docs are embedded as
  comment text in the C++ source code.
  
  **HTML Template.txt** is the frame template being used to embed the contents in each and every HTML file.

## Files generated automatically and to be updated manualls

  **Revolving TOC YYYY.MM.DD hh.mm.ss.csv** manages the table of contents.  This file puts all the different document fragements into one specified sequence
  and with right hierarchical ordering.
  
  Columns:
  Status - Updated by the program: OK, Missing (entry exists, but no docu source found yet), OK yet to integrate (Source found, but category and
  level fields are still blank.
  
  Category - Updated by you: Just 'Body'- Other terms are reserved
  
  Level - Updated by you: 1 (chapter), 2 (section), 3, 4 for further structuring
  
  Section Nr - Updated by the program: Assigns chapter/section number
  
  HTML File Name - Updated by the program
  
  Section Name - Added by the program.  If you change the title name of the text contents, then update the name here, too.  Otherwise, this item will be declared "Missing"
  and a new one being added the bottom of the table as "New" with the new name.
  
  Feature Names - Ipdated by the program: Relates to function names documented in this part, for feature names in generic documentation
  
  Keywords - Updated by the program Additional keywords.  Can be mentioned for cross referencing, e.g. use 2x underscore before and after keyword to mark up with
             automatic cross referencing.
             
  Remarks - Updated by you, will be preserved by the program.  No functional impact.
             
  
  
  
  
  
  
  


## Files generated automatically



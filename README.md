# B4P_Docu_Maker
Utility to create B4P documents


## Required Directories

  **Inputs** contains *enhanced* JSON files with contents not related to specific function names.  All function specific docs are embedded as
  comment text in the C++ source code.
  
  **Images** This subdirectory contains images and other non-HTML files.  The directory with all files will be copied into the destination
  directory where the HTML files are also copied to.
 


## Required files:
  **Build_Docu.b4p** compiles all raw text material and generates all HTML files in the subdirectory "Output".
  Attention: You need to specify the right path to the C source file in order to capture all what you have.  See top of file
  
  **HTML Template.txt** is the frame template being used to embed the contents in each and every HTML file.

  **styles.css** is the style sheet and will be copied into the destination directory along with all HTML files

## Files generated automatically and to be updated manually

  **Revolving TOC YYYY.MM.DD hh.mm.ss.csv** manages the table of contents.  This file puts all the different document fragements into one specified sequence
  and with right hierarchical ordering.  Whenver Docu_Builder.b4p is started, it opens the latest available file, and before done, it will be saved with
  the latest time stamp.  Delete the oldest files if too many files are accumulating here.
  
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

No harm if you delete these files

  **Keyword Index.csv** A table listing all keyowrds
  
  **Example_Program.b4p** All program examples in the docu will be extracted, executed and saved outputs integrated in the docu.  Updated and run several hundred times when processing.
  
  **Example_Out.txt** is the output generated by the Example_Program.b4p.
  
  **Navigator.csv** Supporting file to build the navigator. No need to touch. No harm if deleted
  
  
  
  

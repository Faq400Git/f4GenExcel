# f4GenExcel
IBM i Generate Excel from generic SQL Statement - ILERPG/Node

This is a simple project ILE-RPG and Node.js to generate Excel File from a generic SQL Statement.

There are two steps for the process:

Step 1: Call the F4SQLCOL RPG Program passing your SQL Statement to "describe" the statement, extracting columns headers and columns type, save on a working table wtih a unique id for the SQL Statement

Step 2. Call the node.js app as a web service passing the unique id and the path-name for your excel XSLX file to be generated.


Step by step installation guide:

1) Clone this project in a working IFS directory using an SSH terminal (Putty or similar)
   cd /home
   mkdir F4GenExcel
   
Create a F4SQLCOL0F and F4SQLSTM0F Table in your working library using the SQL Scripts in QSQLSRC direcotry


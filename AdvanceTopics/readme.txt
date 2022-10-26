Assorted Tutorials

# Online Tutorials for Spreadsheet APP (Tutorials 1 -- 9)
  http://edspi31415.blogspot.com/2015/09/hp-prime-spreadsheet-app-tutorial-1-sum.html
  HP Prime Spreadsheet App Tutorial 9: Custom Functions in the Spreadsheet App
  HP Prime Spreadsheet App Tutorial 8: Statistical Analysis
  HP Prime Spreadsheet App Tutorial 6: Row and Column References in Formulas
  
# Plot derivative of a function
I try these example and it works...
F1 : SIN(X)/X
F2 : dF1(X)/dX=X
The key dF1/dX=X just at the right of the catalogue key... will open a pattern menu... 
the partial derivative is on 1rst row and 4th coll...
OR
F1(X)= SIN(X)
F2(X)= SLOPE(F1,X)
where SLOPE() is from Toolbox>App>Function>SLOPE (#5) and
F1 is from Vars>App>Function>Symbolic>F1 (#1)
or type SLOPE(), F1 in with Alpha...

# Plotting a user function?
https://www.hpmuseum.org/forum/thread-641.html
You could:
- assign your equation to V1,V2,.. with a V1:= your_eq_goes_here;
- invoke the advanced graphic application through the STARTAPP("name_of_the_app") command
- uncheck all the other V# with a loop with the command UNCHECK(4); UNCHECK(5),....
UNCHECK({1,2}); //LIST WORKS ON FUNCTION
- invoke the plot screen via STARTVIEW(1);

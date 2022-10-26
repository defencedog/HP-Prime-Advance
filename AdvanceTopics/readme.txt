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

# Spreadsheet and Plotting
One method that seems to have issues now is the following:
- Populate two columns of data in a spreadsheet, say A1:A10 and B1:B10
- Create two user variable lists in two free spreadsheet cells, say xda and yda using =xda:=A1:A10 and =yda:=B1:B10
- Open Statistics2Var Symb view and select xda, yda for S1: data
- Plot, fit data as needed.
OR
In A1-A5, put your data (1,2,3,4,5) and some other data in B1-B5 (1.1,2.3,3.5,4.7,5.1). Now open your stat2var application. Press SYMB.
For your first definition where it currently says C1 for independent, type Spreadsheet.A:A (fully qualified reference to all data in col A of application "Spreadsheet"), for your dependent, type Spreadsheet.B1:B5 (data from B1-B5 in your spreadsheet app).
Now press PLOT and you have what you'd like! Press NUM, STATS to do your stat calculation, etc. Those definitions in symb are not just dumb names, but actual formula locations you can put anything.

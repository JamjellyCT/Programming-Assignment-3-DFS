# Developer Log (DEVLOG.md)
## Depth-First Search

---

### Session 1
**Date:** 2026-04-19
**Task worked on:**
Added parameters to dfs
**Bugs or Issues**
No issues yet.
**Tests**
None yet.
**Fixed or Improved**
Improved parameters, was empty before.



### Session 2
**Date:** 2026-04-19
**Task worked on:**
Added isValid function to check if the current cell position is valid or not.
**Bugs or Issues**
No issues yet.
**Tests**
None yet.
**Fixed or Improved**
Added helper function to clean the DFS implementation.

### Session 3
**Date:** 2026-04-20
**Task worked on:**
dfs function, is able to find E and stop recursion.
**Bugs or Issues**
Printing values using dfs not printing E or S.
Incorrectly setting dfs to false when E was found.
**Tests**
Added print value within dfs to see how it traverses the maze.
**Fixed or Improved**
Changed old if statement within dfs to know detect if the indices are equal
rather than the value itself because E is not actually within the maze which 
I didn't realize.


### Session 4
**Date:** 2026-04-21
**Task worked on:**
dfs function, fixed inccorect return value, added parent tracking
**Bugs or Issues**
Incorrect return value even when E was found.
**Tests**
Added more detail to print cell so I can trace path to see if that was issue.
**Fixed or Improved**
Fixed the recursion within dfs function. dfs didn't return anything so I return dfs if isValid true 
that only made dfs search one path before returning. Fixed the recursion to return proper value
by making another if statement within if valid and making dfs the condition, so that if dfs is true meaning
exit found it would return true.

### Session 5
**Date:** 2026-04-22
**Task worked on:**
testing dfs  and logic
**Bugs or Issues**
No issues from the dfs and logic that I found
Creating a maze with input 1 1 causes program to run indefinitely
**Tests**
Tested different maze sizes, 2 2, 3 3, 4 4, 5 5, 6 6, etc. 
All worked as intended.
If no path found, no path found message displayed, if path found, 
path from entrancee to exit is displayed
**Fixed or Improved**
No improvements rather I proved logic and dfs implementation sound.


### Session 6
**Date:** 2026-04-23
**Task worked on:**
Made 1 1, an invalid input because S and E cannot be at the same spot.
This makes an infinite loop as they keep replacing eachother.
**Bugs or Issues**
Other input   take a long time  because E and S I think are trying to occupy the same spot
Inputs such as 1 2 and 2 1 take a long time because E and S keep trying to occupy the same spot.
Sometimes it works and sometimes it doesn't.
**Tests**
Tested different maze sizes that aren't square such as 2 3, 3 2, 4 2, etc.
**Fixed or Improved**
Program now rejects 1 1 as a valid input as this input causes an infinite loop.

### Session 7
**Date:** 2026-04-24
**Task worked on:**
Created a loop that asks the user for inputs until a valid one is inputted.
Inputs such as 1 1 or inputs with 0 are invalid.
Still need to implement making ints valid inputs. No strings allowed.
**Bugs or Issues**
Inputting a string causes an infinite loop.
**Tests**
Tried inputs such as 1 1, 0 2, 2 0, all loop and prompt the user to input another value.
**Fixed or Improved**
Before the check for inputs 1 1 only did it once so if the user inputted 1 1 again the infinite loop would occur.
Put the check into a while loop so that if an invalid input was inputted it would prompt the user to input again.


### Session 8
**Date:** 2026-04-26
**Task worked on:**
Worked on making input letters invalid. 
**Bugs or Issues**
For current validation checker inputs like e created an infinite loop.
Current implementation is either letter causes error, or inputs like 1 1 creates an error.
Inputs like 3 3e pass. I think cause the way cin works it takes in the inputs like a stream
so it goes in the order of the input so it doesn't reach e. I'll leave it as it doesn't really cause any issues.
**Tests**
Inputs tested like e e, e, 3 e, e 3, 3 3e, 3 3e3, etc. 
**Fixed or Improved**
Now doesn't cause an error when user inputs an letter but the 
validation are still seperate so I need to combine them still.

### Session 9
**Date:** 2026-04-27
**Task worked on:**
Combined validation checkers under one while loop. 
**Bugs or Issues**
Previous validation checker accepted negatives as valid inputs.
I think I covered possible issue / error causing inputs. 
Inputs such as 3 3e pass as the first two values are ints but since the program runs fine I'll intentionally leave it.
**Tests**
Inputs such as: 5 5, 5 e5, e5 5, -4 -2, 3 4-, -4 2, 2 2e
**Fixed or Improved**
Validation for inputs now identifies negatives as invalid inputs. Validation checkers were to seperate while loops
Now validation checkers are within only one loop.


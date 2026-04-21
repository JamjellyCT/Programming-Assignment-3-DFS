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
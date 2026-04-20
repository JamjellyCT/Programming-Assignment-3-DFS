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
# stock_analysis
## Overview of Project
Project manager has requested optimizations to the module controlling the stock application located in the green stocks document. Scope of current task is to refactor existing VBA sub-routine as to only have to read the data table a single time. 

## Results
The refactored code clocks in at around a tenth of second to complete. This is an improvement to the vicinity of half a second that the original code took to complete and sets up the analysis to handle larger volumes of data more efficiently if source dataset was to scale up. 

![before Re-factoring](legacy_2017.png)

![before Re-factoring](legacy_2018.png)

## Summary
 1. The advantage to re-factoring code is that the structure or pattern of the code often comes out cleaner, is more readable, and can be positioned to handle changes to the source data if the schema or volume of data was the change there. This is in addition to any immediate run time advantages. Disadvantages can include introducing competing persepctives on re-factoring - one person's optimization may not be another's, and may not account for patternings that are present elsewhere in other pockets of the project. Additionally while run-time can be saved, the time it takes to refactor will have to borne by some party and it is not always known up front what that time commitment will be.

2. The results speak for themselves in terms of run-time efficieny. Although I was guided through this refactoring all in all it formalized going back through and simply reviewing my work and making changes as needed both to the sub routine and to the parallel commenting. As this sub routine is factored now it is in a better position to work with a shifting, growing data set. The disadvantages flow right along with the above - the time spent on the challenge would be hard to know upfront and as i worked through the refactoring i quickly saw there were nultiple ways i could edit the code under the guise of 'refactoring' and having it still accomplish the task. 

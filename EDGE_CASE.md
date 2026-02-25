# Document your edge case here
- To get marks for this section you will need to explain to your tutor:
1) The edge case you identified
2) How you have accounted for this in your implementation


1) /stats endpoint returns various stats of students' marks, but if there are
no marks or students, then min(), max(), etc. get called on an empty structure.

2) Handled by adding a check at the start of the route and if there are no students,
return a list with null values instead so the program doesn't crash.
System ***specifications*** should be consistent, that is, they should not contain conflicting requirements that could be used to derive a contradiction. When specifications are not consistent, there would be no way to develop a system that satisfies all specifications

Algorithm for checking consistency of a system: **Step 1:** Assign variables to all bits and pieces of specifications. 
**Step 2**: Convert the specifications into logical expressions.
**Step 3**: Construct a truth table containing all the possible combination of the truth values of the total number of variables. 
**Step 4**: Find if there is at least one combination of truth values of the variables such that, all the system specifications turn out to be true.
**Step 5**: If there is such a combination, the system is consistent, otherwise it is inconsistent.

Determine whether these system specifications are consistent: “The diagnostic message is stored in the buffer or it is retransmitted.” “The diagnostic message is not stored in the buffer.” “If the diagnostic message is stored in the buffer, then it is retransmitted.”

Solution: To determine whether these specifications are consistent, we first express them using logical expressions. Let p denote “The diagnostic message is stored in the buffer” and let q denote “The diagnostic message is retransmitted.” The specifications can then be written as p ∨ q, ¬p, and p → q. An assignment of truth values that makes all three specifications true must have p false to make ¬p true. Because we want p ∨ q to be true but p must be false, q must be true. Because p → q is true when p is false and q is true, we conclude that these specifications are consistent, because they are all true when p is false and q is true. We could come to the same conclusion by use of a truth table to examine the four possible assignments of truth values to p and q.


# Haskell Non-Exhaustive Pattern Matching Bug

This repository demonstrates a common error in Haskell: non-exhaustive pattern matching. The `bug.hs` file contains code that only handles the `Just` case of a `Maybe` type, leading to a runtime error when encountering `Nothing`. The `bugSolution.hs` file provides a corrected version.

## How to reproduce

1.  Clone the repository.
2.  Compile `bug.hs` using a Haskell compiler (like GHC).
3.  Run the compiled code, passing `Nothing` as an argument.  Observe the runtime error.
4.  Compile and run `bugSolution.hs` to see the corrected behavior.

## Bug Solution

The solution involves adding a pattern match for the `Nothing` case, handling it appropriately. In this case, we return 0 if the value is `Nothing`.
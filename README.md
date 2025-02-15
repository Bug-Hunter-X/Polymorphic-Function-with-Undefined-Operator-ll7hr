# Haskell Polymorphic Function Error
This repository demonstrates a common Haskell error involving undefined type class instances in polymorphic functions.  The `bug.hs` file contains code that attempts to use the `>` operator on a type variable without specifying an `Ord` instance. This will cause a compile-time error. The solution, demonstrated in `bugSolution.hs`, shows how to constrain the type variable to ensure it has the necessary instance.

**To reproduce the error:**
1.  Compile `bug.hs` using a Haskell compiler (e.g., GHC). You will receive a compile-time error.
2. Compile `bugSolution.hs`. This will compile without errors.
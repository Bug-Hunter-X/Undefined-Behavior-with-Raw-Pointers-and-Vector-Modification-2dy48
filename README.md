# Undefined Behavior with Raw Pointers and Vector Modification in Rust

This repository demonstrates a common error in Rust involving undefined behavior when using raw pointers with vectors. The code attempts to modify a vector's element through a raw pointer after changing its capacity or length. This is unsafe because the vector's internal memory layout might change, leading to unpredictable results.

The `bug.rs` file shows the erroneous code. The `bugSolution.rs` demonstrates a safe approach that avoids undefined behavior by using safe Rust methods to modify the vector. 
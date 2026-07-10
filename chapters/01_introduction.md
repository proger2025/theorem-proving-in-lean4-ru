# 1. Introduction

## 1.1. Computers and Theorem Proving

*Formal verification* involves the use of formal methods to prove the correctness of a program. 
This is different from testing, which only checks a program's behavior on a limited set of inputs.

Lean is a functional programming language and an interactive theorem prover. 
It allows you to write programs and mathematically prove that they satisfy their specifications.

```lean
theorem and_commutative (P Q : Prop) : P ∧ Q → Q ∧ P := by
  intro h
  cases h with
  | intro hp hq =>
    constructor
    · exact hq
    · exact hp
```


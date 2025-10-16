# Combinations and Permutations

A guide to understanding the fundamental difference between combinations and permutations in mathematics.

## Overview

Combinations and permutations are two ways of selecting items from a collection. The key difference lies in whether **order matters**.

- **Permutations**: Order matters
- **Combinations**: Order does not matter

## Permutations

### Definition

A **permutation** is an arrangement of objects in a specific order. When you care about the sequence or position of items, you're dealing with permutations.

### Formula

The number of ways to arrange **r** items from **n** total items:

```
P(n, r) = n! / (n - r)!
```

Where `n!` (n factorial) = n × (n-1) × (n-2) × ... × 2 × 1

### When to Use Permutations

- Arranging people in a line
- Creating passwords where order matters
- Race results (1st, 2nd, 3rd place)
- Seating arrangements
- Lock combinations (ironically!)

### Example

**Question**: How many ways can you arrange 3 books from a shelf of 5 books?

**Solution**:
```
P(5, 3) = 5! / (5 - 3)!
        = 5! / 2!
        = (5 × 4 × 3 × 2 × 1) / (2 × 1)
        = 120 / 2
        = 60
```

**Answer**: 60 different arrangements

**Why?** The book order matters: [Book A, Book B, Book C] is different from [Book C, Book B, Book A].

## Combinations

### Definition

A **combination** is a selection of objects where order does not matter. When you only care about which items are chosen (not their arrangement), you're dealing with combinations.

### Formula

The number of ways to choose **r** items from **n** total items:

```
C(n, r) = n! / (r! × (n - r)!)
```

This is also written as `nCr` or `(n choose r)` or `ⁿCᵣ`.

### When to Use Combinations

- Selecting team members
- Choosing lottery numbers
- Picking pizza toppings
- Forming committees
- Drawing cards from a deck (when order doesn't matter)

### Example

**Question**: How many ways can you choose 3 books from a shelf of 5 books?

**Solution**:
```
C(5, 3) = 5! / (3! × 2!)
        = (5 × 4 × 3 × 2 × 1) / ((3 × 2 × 1) × (2 × 1))
        = 120 / (6 × 2)
        = 120 / 12
        = 10
```

**Answer**: 10 different selections

**Why?** The book order doesn't matter: {Book A, Book B, Book C} is the same as {Book C, Book B, Book A}.

## Key Differences

| Aspect | Permutations | Combinations |
|--------|-------------|--------------|
| **Order** | Matters | Doesn't matter |
| **Formula** | P(n, r) = n! / (n - r)! | C(n, r) = n! / (r! × (n - r)!) |
| **Result** | Arrangements | Selections |
| **Count** | Always ≥ combinations | Always ≤ permutations |
| **Example** | ABC vs BAC are different | ABC and BAC are the same |

## Relationship Between Them

For the same values of n and r:

```
P(n, r) = r! × C(n, r)
```

This makes sense because:
- Combinations tell you how many ways to select items
- For each selection, there are r! ways to arrange those items
- Multiplying gives you the total permutations

## Practical Examples

### Example 1: Pizza Toppings

You can choose 3 toppings from 10 available.

**Use Combinations**: C(10, 3) = 120

The order doesn't matter—pepperoni + mushrooms + olives is the same pizza regardless of which topping you mention first.

### Example 2: Password Creation

You need to create a 4-character password using 4 different letters from the alphabet.

**Use Permutations**: P(26, 4) = 358,800

The order matters—"ABCD" is a different password from "DCBA".

### Example 3: Race Podium

8 runners compete, and you want to know how many different ways the top 3 positions can be filled.

**Use Permutations**: P(8, 3) = 336

The order matters—finishing 1st, 2nd, or 3rd are different outcomes.

### Example 4: Committee Selection

You need to select 5 people from a group of 12 for a committee.

**Use Combinations**: C(12, 5) = 792

The order doesn't matter—the same 5 people form the same committee regardless of selection order.

## Quick Decision Guide

Ask yourself: **"Does order matter?"**

- **YES** → Use Permutations
  - Examples: Rankings, sequences, arrangements, positions
  
- **NO** → Use Combinations
  - Examples: Groups, teams, selections, choices

## Common Mistakes

1. **Confusing the names**: "Combination locks" are actually permutation locks because the order matters!

2. **Not recognizing repeated items**: When items can repeat, different formulas apply.

3. **Forgetting the question context**: Always read carefully to determine if order matters.

## Special Cases

### All items (r = n)

- **Permutations**: P(n, n) = n!
- **Combinations**: C(n, n) = 1 (there's only one way to select everything)

### Selecting none (r = 0)

- **Permutations**: P(n, 0) = 1
- **Combinations**: C(n, 0) = 1

### Symmetry property of combinations

```
C(n, r) = C(n, n - r)
```

Choosing r items to include is the same as choosing (n - r) items to exclude.

## Summary

- **Permutations** count arrangements where **order matters**
- **Combinations** count selections where **order doesn't matter**
- Permutations always give equal or higher counts than combinations for the same n and r
- The relationship: P(n, r) = r! × C(n, r)

Remember: **"Permutation = Position"** and **"Combination = Collection"**

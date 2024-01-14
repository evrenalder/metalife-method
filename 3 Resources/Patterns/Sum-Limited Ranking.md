# Sum-Limited Ranking

## Problem Statement

In decision-making, especially when options are numerous and resources (like time and energy) are limited, prioritizing and choosing the most valuable options becomes challenging.

## Context

This pattern is applicable in situations where you are faced with multiple options and need to make a selection based on a limited capacity for engagement or resources.

![[Sum-Limited-Ranking-Meme.png]]

## Forces

- The need to prioritize among many options.
- Limitations in resources (time, attention, etc.).
- The varying importance or value of each option.

## Solution

Set a maximum limit for the number of items to choose from a larger set. Assign a ranking to each selected item, ensuring that the total of these ranks does not exceed a predetermined sum limit. This encourages thoughtful prioritization based on the perceived value of each option.

## Diagram

![[Sum-Limited-Ranking-Diagram.png]]

## Implementation

1. Determine the maximum number of items to choose (e.g., 10).
2. Set a total sum target for the ranks (e.g., 100).
3. Rank each chosen item, ensuring the sum of ranks equals the target.
4. Balance the ranks across chosen items based on their perceived value.

## Examples

- Prioritizing personal values or goals.
- Allocating a limited budget across different projects.
- Deciding on key features to include in a software release under time constraints.

## Resulting Context

This approach leads to a more manageable set of prioritized options. However, it may also lead to the exclusion of some valuable options due to the imposed limits and may require periodic reevaluation as circumstances change.


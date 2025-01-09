# Elixir List Modification During Enum.each
This example demonstrates an issue related to modifying a list while iterating over it using `Enum.each`.  In Elixir, lists are immutable, so attempting to modify the list in place within the `Enum.each` loop doesn't alter the original list.  This behavior can be surprising to developers coming from languages with mutable lists.

The `bug.exs` file illustrates this issue. The solution, shown in `bugSolution.exs`, demonstrates using `Enum.filter` to correctly achieve the intended result.
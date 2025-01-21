# Kotlin `removeIf` Unexpected Behavior

This example demonstrates a potential issue when using the `removeIf` function on a `MutableList` in Kotlin.  Modifying the list within `removeIf` can lead to unforeseen consequences if you have other references to that list or are concurrently iterating over it.

The `bug.kt` file shows how this can lead to unexpected behavior. The `bugSolution.kt` file offers a safer alternative using an iterator.

This is a common pitfall when working with mutable collections and concurrent modification, highlighting the importance of understanding how these functions affect the original collection.
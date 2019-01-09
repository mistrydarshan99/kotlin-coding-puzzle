# Linked list midpoint

## Nice to solve before
[Linked list](/app/build/tmp/kotlin-classes/debugUnitTest/com/igorwojda/datastructure/linkedlist)

## Instructions

[Puzzle files](.)

Return the 'middle' node of a linked list. If the list has an even number of elements, return
the node at the end of the first half of the list.

We are using version of linked list that implements Kotlin
[Iterator](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-iterator/index.html) interface, so we can use `forEach` instead
of `while` loop.

## Limitations

Do not use a counter variable, do not retrieve the `size` of the list, and only iterate through the list one time.

## Examples

Example 1

```
val l = new LinkedList()
l.insertLast('a')
l.insertLast('b')
l.insertLast('c')
midpoint(l).data // return 'b'
```

Example 2

```
val l = new LinkedList()
l.insertLast('a')
l.insertLast('b')
l.insertLast('c')
l.insertLast('d')
midpoint(l).data // return 'b'
```

## Hints

<details>
<summary>Hint 1</summary>
We should use more then one variable to store values that are retrieved during iteration (two pointer solution)
</details>

<details>
<summary>Hint 2</summary>
Name of these variables should be `slow` and `fast`
</details>

<details>
<summary>Hint 3</summary>
Assign next node to `slow` variable in every iteration
</details>

<details>
<summary>Hint 4</summary>
Assign next node of next node to `fast` variable in every iteration
</details>

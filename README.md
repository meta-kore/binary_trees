# binary_trees

A study of binary trees in C, from a single node up to self-balancing trees, with each stage built on the one before.

All nodes share one type, `binary_tree_t`, aliased as `bst_t`, `avl_t` and `heap_t` depending on the tree being built. Every function is declared in `binary_trees.h`.

## What is in it

| Stage | Functions |
|---|---|
| **Build** | `binary_tree_node`, `binary_tree_insert_left`, `binary_tree_insert_right`, `binary_tree_delete` |
| **Inspect** | `binary_tree_is_leaf`, `binary_tree_is_root`, `binary_tree_height`, `binary_tree_depth`, `binary_tree_size`, `binary_tree_leaves`, `binary_tree_nodes`, `binary_tree_balance`, `binary_tree_sibling`, `binary_tree_uncle`, `binary_trees_ancestor` |
| **Walk** | `binary_tree_preorder`, `binary_tree_inorder`, `binary_tree_postorder`, `binary_tree_levelorder` |
| **Classify** | `binary_tree_is_full`, `binary_tree_is_perfect`, `binary_tree_is_complete`, `binary_tree_is_bst`, `binary_tree_is_avl`, `binary_tree_is_heap` |
| **Rotate** | `binary_tree_rotate_left`, `binary_tree_rotate_right` |
| **Binary search tree** | `bst_insert`, `array_to_bst`, `bst_search`, `bst_remove` |
| **AVL tree** | `avl_insert`, `array_to_avl`, `avl_remove`, `sorted_array_to_avl` |
| **Max binary heap** | `heap_insert`, `array_to_heap`, `heap_extract`, `heap_to_sorted_array` |

The files `115-O`, `125-O` and `135-O` hold the time complexity of the BST, AVL and heap operations.

## Build

`test-files/` has a small `main` for the early functions. Print a tree with `binary_tree_print` and compile with the function under test:

```sh
gcc -Wall -Werror -Wextra -pedantic -std=gnu89 test-files/0-main.c 0-binary_tree_node.c -o node
```

`binary_tree_print` is the course's printing helper and is not in this repository.

## Notes

Built as a project for ALX Africa Software Engineering.

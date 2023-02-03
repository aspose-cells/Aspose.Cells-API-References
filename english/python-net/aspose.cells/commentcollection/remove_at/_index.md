---
title: remove_at method
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 90
url: /python-net/aspose.cells/commentcollection/remove_at/
is_root: false
---

## remove_at(cell_name) {#str}

Removes the comment of the specific cell.



```python
def remove_at(self, cell_name):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| cell_name | str | The name of cell which contains a comment. |

### Example 


```python

comments.remove_at("B2")

```


## remove_at(row, column) {#int-int}

Removes the comment of the specific cell.



```python
def remove_at(self, row, column):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| row | int | The row index. |
| column | int | the column index. |

### Example 


```python

comments.remove_at(1, 1)

```



### See Also
* module [aspose.cells](../../)
* class [CommentCollection](/cells/python-net/aspose.cells/commentcollection)

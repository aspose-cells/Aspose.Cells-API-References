---
title: add_key method
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 20
url: /python-net/aspose.cells/datasorter/add_key/
is_root: false
---

## add_key(key, order) {#int-SortOrder}

Adds sorted column index and sort order.



```python
def add_key(self, key, order):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| key | int | The sorted column index(absolute position, column A is 0, B is 1, ...) |
| order | [SortOrder](/cells/python-net/aspose.cells/sortorder) | The sort order |


## add_key(key, order, custom_list) {#int-SortOrder-str}

Adds sorted column index and sort order with custom sort list.



```python
def add_key(self, key, order, custom_list):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| key | int | The sorted column index(absolute position, column A is 0, B is 1, ...) |
| order | [SortOrder](/cells/python-net/aspose.cells/sortorder) | The sort order. |
| custom_list | str | The custom sort list. |


## add_key(key, order, custom_list) {#int-SortOrder-list}



```python
def add_key(self, key, order, custom_list):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| key | int |  |
| order | [SortOrder](/cells/python-net/aspose.cells/sortorder) |  |
| custom_list | list |  |


## add_key(key, type, order, custom_list) {#int-SortOnType-SortOrder-any}

Adds sorted column index and sort order with custom sort list.



```python
def add_key(self, key, type, order, custom_list):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| key | int | The sorted column index(absolute position, column A is 0, B is 1, ...) |
| type | [SortOnType](/cells/python-net/aspose.cells/sortontype) | The sorted value type. |
| order | [SortOrder](/cells/python-net/aspose.cells/sortorder) | The sort order. |
| custom_list | any | The custom sort list. |
### Remarks

If type is SortOnType.CellColor or SortOnType.FontColor, the customList is Color.


### See Also
* module [aspose.cells](../../)
* class [DataSorter](/cells/python-net/aspose.cells/datasorter)

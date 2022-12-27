---
title: remove_at method
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 40
url: /python-net/aspose.cells/externallinkcollection/remove_at/
is_root: false
---

## remove_at(index) {#int}

Removes the specified external link from the workbook.



```python
def remove_at(self, index):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| index | int | the index of the external link to be removed. |
### Remarks

When removing the external link, all formulas that reference to it will be removed too because
the references become invalid.

## remove_at(index, update_references_as_local) {#int-bool}

Removes the specified external link from the workbook.



```python
def remove_at(self, index, update_references_as_local):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| index | int | the index of the external link to be removed. |
| update_references_as_local | bool | Whether update all references of given external link to reference of current workbook itself. |
### Remarks

If references are required to be updated, references to external links in formulas will be changed to current workbook.
For example, the external link to be removed is "externalsource.xlam" and it defines one custom function "customfunction()",
one cell's original formula is "='externalsource.xlam'!customfunction()",
after removing the formula will become "=customfunction()".
If reference are not required to be updated, all formulas with reference to this external link
will be removed too because those references become invalid.


### See Also
* module [aspose.cells](../../)
* class [ExternalLinkCollection](/cells/python-net/aspose.cells/externallinkcollection)

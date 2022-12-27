---
title: clear method
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 30
url: /python-net/aspose.cells/externallinkcollection/clear/
is_root: false
---

## clear() {#}

Removes all external links.



```python
def clear(self):
    ...
```


### Remarks

When removing external links, all formulas that reference to them will be removed too because
the references become invalid.

## clear(update_references_as_local) {#bool}

Removes all external links.



```python
def clear(self, update_references_as_local):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| update_references_as_local | bool | Whether update all references of external links as references of current workbook itself. |
### Remarks

If references are required to be updated, references to external links in formulas will be changed to current workbook.
For example, one cell's original formula is "='externalsource.xlam'!customfunction()",
after removing external links, the formula will become "=customfunction()".
If references are not required to be updated, all formulas with references to external links
will be removed too because those references become invalid.


### See Also
* module [aspose.cells](../../)
* class [ExternalLinkCollection](/cells/python-net/aspose.cells/externallinkcollection)

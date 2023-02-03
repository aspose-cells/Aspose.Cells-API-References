---
title: get_enumerator method
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 40
url: /python-net/aspose.cells/unionrange/get_enumerator/
is_root: false
---

## get_enumerator() {#}

Gets the enumerator for cells in this Range.


### Returns 


The cells enumerator


```python
def get_enumerator(self):
    ...
```


### Remarks

When traversing elements by the returned Enumerator, the cells collection
should not be modified(such as operations that will cause new Cell/Row be instantiated or existing Cell/Row be deleted).
Otherwise the enumerator may not be able to traverse all cells correctly(some elements may be traversed repeatedly or skipped).


### See Also
* module [aspose.cells](../../)
* class [UnionRange](/cells/python-net/aspose.cells/unionrange)

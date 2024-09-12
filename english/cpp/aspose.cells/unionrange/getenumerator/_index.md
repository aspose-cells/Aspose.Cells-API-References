---
title: Aspose::Cells::UnionRange::GetEnumerator method
linktitle: GetEnumerator
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::UnionRange::GetEnumerator method. Gets the enumerator for cells in this Range in C++.'
type: docs
weight: 2300
url: /cpp/aspose.cells/unionrange/getenumerator/
---
## UnionRange::GetEnumerator method


Gets the enumerator for cells in this [Range](../../range/).

```cpp
Enumerator<Cell> Aspose::Cells::UnionRange::GetEnumerator()
```


## ReturnValue

The cells enumerator
## Remarks



When traversing elements by the returned [Enumerator](../../enumerator/), the cells collection should not be modified(such as operations that will cause new Cell/Row be instantiated or existing Cell/Row be deleted). Otherwise the enumerator may not be able to traverse all cells correctly(some elements may be traversed repeatedly or skipped).
## See Also

* Class [Enumerator](../../enumerator/)
* Class [Cell](../../cell/)
* Class [UnionRange](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)

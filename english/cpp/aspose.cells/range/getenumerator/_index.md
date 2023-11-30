---
title: Aspose::Cells::Range::GetEnumerator method
linktitle: GetEnumerator
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Range::GetEnumerator method. Gets the enumerator for cells in this Range in C++.'
type: docs
weight: 1000
url: /cpp/aspose.cells/range/getenumerator/
---
## Range::GetEnumerator method


Gets the enumerator for cells in this [Range](../).

```cpp
Enumerator<Cell> Aspose::Cells::Range::GetEnumerator()
```


## ReturnValue

The cells enumerator
## Remarks



When traversing elements by the returned [Enumerator](../../enumerator/), the cells collection should not be modified(such as operations that will cause new Cell/Row be instantiated or existing Cell/Row be deleted). Otherwise the enumerator may not be able to traverse all cells correctly(some elements may be traversed repeatedly or skipped).

## Examples


```cpp
Aspose::Cells::Startup();
Workbook workbook(u"template.xlsx");
Cells cells = workbook.GetWorksheets().Get(0).GetCells();

Enumerator<Cell> en = cells.CreateRange(u"B2:C3").GetEnumerator();
while (en.MoveNext())
{
    Cell cell = (Cell)en.GetCurrent();
    std::cout << cell.GetName().ToUtf8() << std::endl;
}
Aspose::Cells::Cleanup();
```

## See Also

* Class [Enumerator](../../enumerator/)
* Class [Cell](../../cell/)
* Class [Range](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)

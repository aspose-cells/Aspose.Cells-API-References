---
title: Aspose::Cells::Cells::DeleteBlankRows method
linktitle: DeleteBlankRows
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Cells::DeleteBlankRows method. Delete all blank rows which do not contain any data or other object in C++.'
type: docs
weight: 11400
url: /cpp/aspose.cells/cells/deleteblankrows/
---
## Cells::DeleteBlankRows() method


Delete all blank rows which do not contain any data or other object.

```cpp
void Aspose::Cells::Cells::DeleteBlankRows()
```

## See Also

* Class [Vector](../../vector/)
* Class [Cells](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## Cells::DeleteBlankRows(const DeleteOptions\&) method


Delete all blank rows which do not contain any data or other object.

```cpp
void Aspose::Cells::Cells::DeleteBlankRows(const DeleteOptions &options)
```


| Parameter | Type | Description |
| --- | --- | --- |
| options | const DeleteOptions\& | The options of deleting range. |
## Remarks



For blank rows that will be deleted, it is not only required that [Row.IsBlank](../../row/isblank/) should be true, but also there should be no visible comment defined for any cell in those rows, and no pivot table whose range intersects with them. 
## See Also

* Class [Vector](../../vector/)
* Class [DeleteOptions](../../deleteoptions/)
* Class [Cells](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)

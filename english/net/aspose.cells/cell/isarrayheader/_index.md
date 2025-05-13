---
title: Cell.IsArrayHeader
second_title: Aspose.Cells for .NET API Reference
description: Cell property. Indicates the cells formula is an array formula and it is the first cell of the array
type: docs
url: /net/aspose.cells/cell/isarrayheader/
---
## Cell.IsArrayHeader property

Indicates the cell's formula is an array formula and it is the first cell of the array.

```csharp
public bool IsArrayHeader { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(workbook.Worksheets[0].Cells["C31"].IsArrayHeader, true);
public void Cell_Property_IsArrayHeader()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xml");
    Assert.AreEqual(workbook.Worksheets[0].Cells["C31"].IsArrayHeader, true);
}
```

### See Also

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



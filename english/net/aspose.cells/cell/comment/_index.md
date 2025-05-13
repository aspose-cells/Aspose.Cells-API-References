---
title: Cell.Comment
second_title: Aspose.Cells for .NET API Reference
description: Cell property. Gets the comment of this cell
type: docs
url: /net/aspose.cells/cell/comment/
---
## Cell.Comment property

Gets the comment of this cell.

```csharp
public Comment Comment { get; }
```

### Remarks

If there is no comment applies to the cell, returns null.

### Examples

```csharp
// Called: Assert.NotNull(d10.Comment);
public void Cell_Property_Comment()
{
    Workbook wb = new Workbook(Constants.sourcePath + @"example.numbers");
    Cells cells = wb.Worksheets[0].Cells;
    Cell d10 = cells["D10"];
    Assert.AreEqual("=COUNT(A1:A10)", d10.Formula);
    Assert.AreEqual("0.00\\ ", d10.GetStyle().Custom);//0.00_ 
    Assert.AreEqual(0, d10.GetStyle().Number);
    Assert.NotNull(d10.Comment);
    Cell c11 = cells["C11"];
}
```

### See Also

* class [Comment](../../comment/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



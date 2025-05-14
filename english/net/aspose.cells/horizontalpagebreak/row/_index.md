---
title: HorizontalPageBreak.Row
second_title: Aspose.Cells for .NET API Reference
description: HorizontalPageBreak property. Gets the zero based row index
type: docs
url: /net/aspose.cells/horizontalpagebreak/row/
---
## HorizontalPageBreak.Row property

Gets the zero based row index.

```csharp
public int Row { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(6, breaks[0].Row);
public void HorizontalPageBreak_Property_Row()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    HorizontalPageBreakCollection breaks = workbook.Worksheets[0].HorizontalPageBreaks;
    Assert.AreEqual(2, breaks.Count);
    Assert.AreEqual(6, breaks[0].Row);
    Assert.AreEqual(12, breaks[1].Row);
    workbook.Save(Constants.destPath + "example.ods");
    workbook = new Workbook(Constants.destPath + "example.ods");
     breaks = workbook.Worksheets[0].HorizontalPageBreaks;
    Assert.AreEqual(2, breaks.Count);
    Assert.AreEqual(6, breaks[0].Row);
    Assert.AreEqual(12, breaks[1].Row);
    workbook.Save(Constants.destPath + "example.xlsx");
}
```

### See Also

* class [HorizontalPageBreak](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



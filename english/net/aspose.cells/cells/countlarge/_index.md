---
title: Cells.CountLarge
second_title: Aspose.Cells for .NET API Reference
description: Cells property. Gets the total count of instantiated Cell objects
type: docs
url: /net/aspose.cells/cells/countlarge/
---
## Cells.CountLarge property

Gets the total count of instantiated Cell objects.

```csharp
public long CountLarge { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(1, workbook.Worksheets[0].Cells.CountLarge);
public void Cells_Property_CountLarge()
{
           
    Workbook workbook = new Workbook();
    workbook.Worksheets[0].Cells["A4"].PutValue("test");
    Assert.AreEqual(1, workbook.Worksheets[0].Cells.CountLarge);
    PageSetup setup = workbook.Worksheets[0].PageSetup;
   Assert.AreEqual(11,setup.PaperHeight);
    Assert.AreEqual(8.5, setup.PaperWidth);
}
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



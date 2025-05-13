---
title: Worksheet.Cells
second_title: Aspose.Cells for .NET API Reference
description: Worksheet property. Gets the Cells collection
type: docs
url: /net/aspose.cells/worksheet/cells/
---
## Worksheet.Cells property

Gets the `Cells` collection.

```csharp
public Cells Cells { get; }
```

### Examples

```csharp
// Called: Cells cells = wb.Worksheets[0].Cells;
public void Worksheet_Property_Cells()
{
    //formula(range) error
    Workbook wb = new Workbook(Constants.sourcePath + "example.numbers");
    wb = Util.ReSave(wb, SaveFormat.Xlsx);
    Cells cells = wb.Worksheets[0].Cells;
    Assert.AreEqual("3976.2", cells["E31"].StringValue);
    Assert.AreEqual("=SUM(E3:E29)", cells["E31"].Formula);
    Assert.AreEqual("166", cells["E3"].StringValue);
    Assert.AreEqual("79.8", cells["E29"].StringValue);
    Assert.AreEqual("170", cells["C23"].StringValue);
    Assert.AreEqual("2.66", cells["D13"].StringValue);
    //check foregroundColor for the first line and row...

}
```

### See Also

* class [Cells](../../cells/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



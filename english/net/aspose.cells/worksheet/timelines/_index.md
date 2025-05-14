---
title: Worksheet.Timelines
second_title: Aspose.Cells for .NET API Reference
description: Worksheet property. Get the Timeline collection in the worksheet
type: docs
url: /net/aspose.cells/worksheet/timelines/
---
## Worksheet.Timelines property

Get the Timeline collection in the worksheet

```csharp
public TimelineCollection Timelines { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(sheet.Timelines.Count, 1);
public void Worksheet_Property_Timelines()
{
    string filePath = Constants.PivotTableSourcePath + "JAVA44320_";
    string savePath = CreateFolder(filePath);

    Workbook wb = new Workbook(filePath + "a.xlsx");
    Worksheet sheet = wb.Worksheets[1];
    PivotTable pivot = sheet.PivotTables[0];
    sheet.Timelines.Add(pivot, 8, 8, "Ship Date");

    Assert.AreEqual(sheet.Shapes.Count, 1);
    Assert.AreEqual(sheet.Timelines.Count, 1);
    wb.Save(savePath + "out.xlsx");
}
```

### See Also

* class [TimelineCollection](../../../aspose.cells.timelines/timelinecollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



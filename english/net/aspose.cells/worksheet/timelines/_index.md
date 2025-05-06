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
// Called: sheet.Timelines.Add(pivot, 8, 8, &amp;quot;Ship Date&amp;quot;);
[Test]
        public void Property_Timelines()
        {
            string filePath = Constants.PivotTableSourcePath + &quot;JAVA44320_&quot;;
            string savePath = CreateFolder(filePath);

            Workbook wb = new Workbook(filePath + &quot;a.xlsx&quot;);
            Worksheet sheet = wb.Worksheets[1];
            PivotTable pivot = sheet.PivotTables[0];
            sheet.Timelines.Add(pivot, 8, 8, &quot;Ship Date&quot;);

            Assert.AreEqual(sheet.Shapes.Count, 1);
            Assert.AreEqual(sheet.Timelines.Count, 1);
            wb.Save(savePath + &quot;out.xlsx&quot;);
        }
```

### See Also

* class [TimelineCollection](../../../aspose.cells.timelines/timelinecollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



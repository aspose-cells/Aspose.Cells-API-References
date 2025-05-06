---
title: Style.ForegroundArgbColor
second_title: Aspose.Cells for .NET API Reference
description: Style property. Gets and sets the foreground color with a 32bit ARGB value
type: docs
url: /net/aspose.cells/style/foregroundargbcolor/
---
## Style.ForegroundArgbColor property

Gets and sets the foreground color with a 32-bit ARGB value.

```csharp
public int ForegroundArgbColor { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(cells[&amp;quot;D26&amp;quot;].GetStyle().ForegroundArgbColor, 0);
[Test]
        public void Property_ForegroundArgbColor()
        {
            string filePath = Constants.PivotTableSourcePath + @&quot;NET46410_&quot;;

            Workbook sourceWorkbook = new Workbook(filePath + @&quot;DemoForAspose.xlsx&quot;);
            foreach (Worksheet workbookWorksheet in sourceWorkbook.Worksheets)
            {
                foreach (PivotTable workbookWorksheetPivotTable in workbookWorksheet.PivotTables)
                {
                    workbookWorksheetPivotTable.RefreshData();
                    workbookWorksheetPivotTable.CalculateData();
                }
            }
           // sourceWorkbook.Save(CreateFolder(filePath) + @&quot;out.html&quot;);
            Cells cells = sourceWorkbook.Worksheets[&quot;ABS&quot;].Cells;
            Assert.AreEqual(cells[&quot;D24&quot;].GetStyle().ForegroundArgbColor, 0);
            Assert.AreEqual(cells[&quot;D26&quot;].GetStyle().ForegroundArgbColor, 0);

            sourceWorkbook.Worksheets.RemoveAt(&quot;Limits Export&quot;);

           
        }
```

### See Also

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



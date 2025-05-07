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
// Called: Assert.AreEqual(cells["D24"].GetStyle().ForegroundArgbColor, 0);
[Test]
        public void Property_ForegroundArgbColor()
        {
            string filePath = Constants.PivotTableSourcePath + @"NET46410_";

            Workbook sourceWorkbook = new Workbook(filePath + @"DemoForAspose.xlsx");
            foreach (Worksheet workbookWorksheet in sourceWorkbook.Worksheets)
            {
                foreach (PivotTable workbookWorksheetPivotTable in workbookWorksheet.PivotTables)
                {
                    workbookWorksheetPivotTable.RefreshData();
                    workbookWorksheetPivotTable.CalculateData();
                }
            }
           // sourceWorkbook.Save(CreateFolder(filePath) + @"out.html");
            Cells cells = sourceWorkbook.Worksheets["ABS"].Cells;
            Assert.AreEqual(cells["D24"].GetStyle().ForegroundArgbColor, 0);
            Assert.AreEqual(cells["D26"].GetStyle().ForegroundArgbColor, 0);

            sourceWorkbook.Worksheets.RemoveAt("Limits Export");

           
        }
```

### See Also

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



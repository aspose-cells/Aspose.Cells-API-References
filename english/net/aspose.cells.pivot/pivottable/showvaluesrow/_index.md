---
title: PivotTable.ShowValuesRow
second_title: Aspose.Cells for .NET API Reference
description: PivotTable property. Indicates whether showing values row
type: docs
url: /net/aspose.cells.pivot/pivottable/showvaluesrow/
---
## PivotTable.ShowValuesRow property

Indicates whether showing values row.

```csharp
public bool ShowValuesRow { get; set; }
```

### Examples

```csharp
// Called: Console.WriteLine("Before " + table.ShowValuesRow);
[Test]
        public void Property_ShowValuesRow()
        {
            string filePath = Constants.PivotTableSourcePath + @"NET46650_";

            Workbook workbook = new Workbook(filePath + @"origin.xlsx");

            foreach (Worksheet sheet in workbook.Worksheets)
            {
                foreach (PivotTable table in sheet.PivotTables)
                {
                    Console.WriteLine("Before " + table.ShowValuesRow);
                    table.ShowValuesRow = false;
                    Console.WriteLine("After " + table.ShowValuesRow);
                }
                sheet.RefreshPivotTables();
            }

            workbook.Save(CreateFolder(filePath) + @"out.xlsx", Aspose.Cells.SaveFormat.Xlsx);

            workbook = new Workbook(CreateFolder(filePath) + @"out.xlsx");
            Assert.AreEqual(workbook.Worksheets[0].PivotTables[0].ShowValuesRow, false);
        }
```

### See Also

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)



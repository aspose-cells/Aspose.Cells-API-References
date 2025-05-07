---
title: Worksheet.PivotTables
second_title: Aspose.Cells for .NET API Reference
description: Worksheet property. Gets all pivot tables in this worksheet
type: docs
url: /net/aspose.cells/worksheet/pivottables/
---
## Worksheet.PivotTables property

Gets all pivot tables in this worksheet.

```csharp
public PivotTableCollection PivotTables { get; }
```

### Examples

```csharp
// Called: PivotTable table = wb.Worksheets[1].PivotTables[0];
[Test]
        public void Property_PivotTables()
        {
            string filePath = Constants.PivotTableSourcePath + @"JAVA41098_";
            Workbook wb = new Workbook(filePath + "testExcel.xlsx");
            PivotTable table = wb.Worksheets[1].PivotTables[0];
            table.PreserveFormatting = true;
            table.RefreshData();
            table.CalculateData();
            Cells cells = wb.Worksheets[1].Cells;
            Assert.AreNotEqual(cells["C6"].StringValue.IndexOf("%"), -1);
            Assert.AreNotEqual(cells["D6"].StringValue.IndexOf("%"), -1);
            wb.Save(Constants.PivotTableDestPath + @"JAVA41098.pdf", SaveFormat.Pdf);
        }
```

### See Also

* class [PivotTableCollection](../../../aspose.cells.pivot/pivottablecollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



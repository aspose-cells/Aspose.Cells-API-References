---
title: WorksheetCollection.ClearPivottables
second_title: Aspose.Cells for .NET API Reference
description: WorksheetCollection method. Clears pivot tables from the spreadsheet
type: docs
url: /net/aspose.cells/worksheetcollection/clearpivottables/
---
## WorksheetCollection.ClearPivottables method

Clears pivot tables from the spreadsheet.

```csharp
public void ClearPivottables()
```

### Examples

```csharp
// Called: workbook.Worksheets.ClearPivottables();
[Test]
        public void Method_ClearPivottables()
        {
            Workbook workbook = new Workbook(Constants.PivotTableSourcePath + &quot;CELLSNET44380.xlsx&quot;);
            workbook.Worksheets.ClearPivottables();
            Assert.AreEqual(0, workbook.Worksheets[0].PivotTables.Count);
            workbook.Save(Constants.PivotTableDestPath + &quot;CELLSNET44380.xlsx&quot;);
        }
```

### See Also

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



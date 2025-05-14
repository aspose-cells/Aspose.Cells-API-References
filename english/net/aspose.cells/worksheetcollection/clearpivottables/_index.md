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
public void WorksheetCollection_Method_ClearPivottables()
{
    Workbook workbook = new Workbook(Constants.PivotTableSourcePath + "example.xlsx");
    workbook.Worksheets.ClearPivottables();
    Assert.AreEqual(0, workbook.Worksheets[0].PivotTables.Count);
    workbook.Save(Constants.PivotTableDestPath + "example.xlsx");
}
```

### See Also

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



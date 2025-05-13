---
title: WorksheetCollection.GetSheetByCodeName
second_title: Aspose.Cells for .NET API Reference
description: WorksheetCollection method. Gets the worksheet by the code name
type: docs
url: /net/aspose.cells/worksheetcollection/getsheetbycodename/
---
## WorksheetCollection.GetSheetByCodeName method

Gets the worksheet by the code name.

```csharp
public Worksheet GetSheetByCodeName(string codeName)
```

| Parameter | Type | Description |
| --- | --- | --- |
| codeName | String | Worksheet code name. |

### Return Value

The element with the specified code name.

### Examples

```csharp
// Called: Worksheet pivotTableSheet = workbook.Worksheets.GetSheetByCodeName("Pvt");
public void WorksheetCollection_Method_GetSheetByCodeName()
{
    var workbook = new Workbook(Constants.openPivottablePath + "Template.xlsx");
    Worksheet pivotTableSheet = workbook.Worksheets.GetSheetByCodeName("Pvt");
    Worksheet dataFinalSheet = workbook.Worksheets.GetSheetByCodeName("DataFinal");
    PivotTable pivotTable = pivotTableSheet.PivotTables[0];
    Aspose.Cells.Range range = dataFinalSheet.Cells.CreateRange(0, 0, dataFinalSheet.Cells.MaxDataRow + 1, dataFinalSheet.Cells.MaxColumn);
    range.Name = "MngfulDiffAnalysisDataSource";
    pivotTable.RefreshData();
    workbook.Save(Constants.savePivottablePath + "OutPivotTable1.xlsx");

}
```

### See Also

* class [Worksheet](../../worksheet/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



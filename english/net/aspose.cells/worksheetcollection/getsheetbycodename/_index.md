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
// Called: Worksheet pivotTableSheet = workbook.Worksheets.GetSheetByCodeName(&amp;quot;Pvt&amp;quot;);
[Test]
        public void Method_String_()
        {
            var workbook = new Workbook(Constants.openPivottablePath + &quot;Template.xlsx&quot;);
            Worksheet pivotTableSheet = workbook.Worksheets.GetSheetByCodeName(&quot;Pvt&quot;);
            Worksheet dataFinalSheet = workbook.Worksheets.GetSheetByCodeName(&quot;DataFinal&quot;);
            PivotTable pivotTable = pivotTableSheet.PivotTables[0];
            Aspose.Cells.Range range = dataFinalSheet.Cells.CreateRange(0, 0, dataFinalSheet.Cells.MaxDataRow + 1, dataFinalSheet.Cells.MaxColumn);
            range.Name = &quot;MngfulDiffAnalysisDataSource&quot;;
            pivotTable.RefreshData();
            workbook.Save(Constants.savePivottablePath + &quot;OutPivotTable1.xlsx&quot;);

        }
```

### See Also

* class [Worksheet](../../worksheet/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



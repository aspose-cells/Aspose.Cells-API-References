---
title: PivotTable.GetCellByDisplayName
second_title: Aspose.Cells for .NET API Reference
description: PivotTable method. Gets the Cell object by the display name of PivotField
type: docs
url: /net/aspose.cells.pivot/pivottable/getcellbydisplayname/
---
## PivotTable.GetCellByDisplayName method

Gets the [`Cell`](../../../aspose.cells/cell/) object by the display name of PivotField.

```csharp
public Cell GetCellByDisplayName(string displayName)
```

| Parameter | Type | Description |
| --- | --- | --- |
| displayName | String | the DisplayName of PivotField |

### Return Value

the Cell object

### Examples

```csharp
// Called: var cell = pivotTable.GetCellByDisplayName(column);
private static void Method_String_(Workbook workbook, List<string> columns)
        {
            var pivotSheet = workbook.Worksheets.Add("Pivot1");
            var pivotTableIndex = pivotSheet.PivotTables.Add(string.Format("'{0}'!{1}", "Pivot1", "Data0"), "A5", "Pivot");
            var pivotTable = pivotSheet.PivotTables[pivotTableIndex];
            foreach (var column in columns)
            {
                pivotTable.AddFieldToArea(PivotFieldType.Row, column);
            }
            pivotTable.CalculateData();

            foreach (var column in columns)
            {
                var cell = pivotTable.GetCellByDisplayName(column);
                if (cell == null)
                    continue;
                var style = new Style(); // this used to work in 20.04 but causes corruption starting with 20.06
                                         // style.BackgroundColor = Color.Red;
                pivotTable.Format(cell.Row, cell.Column, style);
            }
        }
```

### See Also

* class [Cell](../../../aspose.cells/cell/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)



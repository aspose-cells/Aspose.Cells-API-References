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
// Called: Cell cell = pivotTable.GetCellByDisplayName(pivotTable.DataFields[2].DisplayName);
[Test]
        public void Method_String_()
        {
            string filePath = Constants.PivotTableSourcePath + @&quot;NET43367_&quot;;
            var workbook = new Workbook(filePath + &quot;example2.xlsx&quot;);
            var worksheet = workbook.Worksheets[0];
            var pivotTable = worksheet.PivotTables[0];

            pivotTable.RefreshData();
            pivotTable.CalculateData();
            pivotTable.RefreshDataOnOpeningFile = false;

            Style style = workbook.CreateStyle();
            style.BackgroundColor = Color.Yellow;
            style.Pattern = BackgroundType.Solid;
            Cell cell = pivotTable.GetCellByDisplayName(pivotTable.DataFields[2].DisplayName);

            int preColor = cell.GetStyle().ForegroundArgbColor;
            pivotTable.Format(cell.Row, cell.Column, style);
            Assert.AreNotEqual(preColor, cell.GetStyle().ForegroundArgbColor);
            workbook.Save(Constants.PivotTableDestPath + @&quot;NET43367.xlsx&quot;);
        }
```

### See Also

* class [Cell](../../../aspose.cells/cell/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)



---
title: PivotTable.Format
second_title: Aspose.Cells for .NET API Reference
description: PivotTable method. Formats selected area of the PivotTable
type: docs
url: /net/aspose.cells.pivot/pivottable/format/
---
## Format(PivotArea, Style) {#format_1}

Formats selected area of the PivotTable.

```csharp
public void Format(PivotArea pivotArea, Style style)
```

| Parameter | Type | Description |
| --- | --- | --- |
| pivotArea | PivotArea | The selected pivot view area. |
| style | Style | The formatted setting. |

### See Also

* class [PivotArea](../../pivotarea/)
* class [Style](../../../aspose.cells/style/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Format(CellArea, Style) {#format}

Formats selected area of the PivotTable.

```csharp
public void Format(CellArea ca, Style style)
```

| Parameter | Type | Description |
| --- | --- | --- |
| ca | CellArea | The range of the cells. |
| style | Style | The style |

### See Also

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [Style](../../../aspose.cells/style/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Format(int, int, Style) {#format_2}

Format the cell in the pivottable area

```csharp
public void Format(int row, int column, Style style)
```

| Parameter | Type | Description |
| --- | --- | --- |
| row | Int32 | Row Index of the cell |
| column | Int32 | Column index of the cell |
| style | Style | Style which is to format the cell |

### Examples

```csharp
// Called: pivotTable.Format(cell.Row, cell.Column, style);
private static void PivotTable_Method_Format(Workbook workbook, List<string> columns)
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

* class [Style](../../../aspose.cells/style/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)



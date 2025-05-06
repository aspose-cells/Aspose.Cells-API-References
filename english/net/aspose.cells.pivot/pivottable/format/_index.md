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
// Called: wb.Worksheets[2].PivotTables[0].Format(10, 0, style);
[Test]
        public void Method_Style_()
        {

            Workbook wb = new Workbook(Constants.openPivottablePath + &quot;Source.xlsx&quot;);
            Style style = wb.CreateStyle();
            style.Custom = &quot;dd/mmm&quot;;
            wb.Worksheets[2].PivotTables[0].Format(9, 0, style);
            wb.Worksheets[2].PivotTables[0].Format(10, 0, style);
            wb.Worksheets[2].PivotTables[0].Format(11, 0, style);
            wb.Worksheets[2].PivotTables[0].Format(12, 0, style);
            wb.Worksheets[2].PivotTables[0].RowFields[0].IsAutoSubtotals = false;
            wb.Worksheets[2].PivotTables[0].RowFields[0].ShowInOutlineForm = false;
            wb.Worksheets[2].PivotTables[0].RefreshData();
            wb.Worksheets[2].PivotTables[0].CalculateData();
            wb.Save(Constants.savePivottablePath + &quot;40013.xlsx&quot;);
        }
```

### See Also

* class [Style](../../../aspose.cells/style/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)



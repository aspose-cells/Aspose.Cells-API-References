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
[Test]
        public void Method_Style_()
        {
            string filePath = Constants.PivotTableSourcePath + @"NET43367_";
            var workbook = new Workbook(filePath + "example2.xlsx");
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
            workbook.Save(Constants.PivotTableDestPath + @"NET43367.xlsx");
        }
```

### See Also

* class [Style](../../../aspose.cells/style/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)



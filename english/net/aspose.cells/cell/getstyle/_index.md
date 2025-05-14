---
title: Cell.GetStyle
second_title: Aspose.Cells for .NET API Reference
description: Cell method. Gets the cell style
type: docs
url: /net/aspose.cells/cell/getstyle/
---
## GetStyle() {#getstyle}

Gets the cell style.

```csharp
public Style GetStyle()
```

### Return Value

Style object.

### Remarks

To change the style of the cell, please call Cell.SetStyle() method after modifying the returned style object. This method is same with `GetStyle` with true value for the parameter.

### Examples

```csharp
// Called: testAreEqual(TextAlignmentType.Top, cells[4, 0].GetStyle().VerticalAlignment, caseName);
private void Cell_Method_GetStyle(Workbook workbook)
        {
            Cells cells = workbook.Worksheets[0].Cells;
            testAreEqual(TextAlignmentType.Bottom, cells[0, 0].GetStyle().VerticalAlignment, caseName);
            testAreEqual(TextAlignmentType.Center, cells[1, 0].GetStyle().VerticalAlignment, caseName);
            testAreEqual(TextAlignmentType.Distributed, cells[2, 0].GetStyle().VerticalAlignment, caseName);
            testAreEqual(TextAlignmentType.Justify, cells[3, 0].GetStyle().VerticalAlignment, caseName);
            testAreEqual(TextAlignmentType.Top, cells[4, 0].GetStyle().VerticalAlignment, caseName);
        }
```

### See Also

* class [Style](../../style/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetStyle(bool) {#getstyle_1}

If checkBorders is true, check whether other cells' borders will effect the style of this cell.

```csharp
public Style GetStyle(bool checkBorders)
```

| Parameter | Type | Description |
| --- | --- | --- |
| checkBorders | Boolean | Check other cells' borders |

### Return Value

Style object.

### Examples

```csharp
// Called: Assert.AreEqual(cell.GetStyle(false).Borders[BorderType.TopBorder].LineStyle, CellBorderType.None);
public void Cell_Method_GetStyle()
{

    var workbook = new Workbook(Constants.sourcePath + @"example.xlsx");
    var fromRange = workbook.Worksheets[0].Cells.CreateRange(1, 0, 5, 1).EntireRow; // copy rows 1 - 10
    var toRange = workbook.Worksheets[1].Cells.CreateRange(11, 0, 1, 1);

    toRange.Copy(fromRange); // copy the data from the range
    int iLastRow = fromRange.FirstRow + fromRange.RowCount;
    int iLastCol = fromRange.FirstColumn + fromRange.ColumnCount;
    for (int iRow = fromRange.FirstRow; iRow < iLastRow; iRow++)
    {
        for (int iCol = fromRange.FirstColumn; iCol < iLastCol; iCol++)
        {
            Cell cell = workbook.Worksheets[0].Cells[iRow, iCol];
            var style = cell.GetStyle(false);
            style.Custom = "0.000";

            var styleFlag = new StyleFlag();
            styleFlag.NumberFormat = true; // only number format should be changed
            cell.SetStyle(style, styleFlag);

            Assert.AreEqual(cell.GetStyle(false).Borders[BorderType.TopBorder].LineStyle, CellBorderType.None);
        }

    }
    toRange.Copy(fromRange); // copy the data from the range
    workbook.Save(Constants.destPath + @"example.xlsx");
}
```

### See Also

* class [Style](../../style/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



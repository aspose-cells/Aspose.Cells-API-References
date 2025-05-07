---
title: Cell.SetStyle
second_title: Aspose.Cells for .NET API Reference
description: Cell method. Sets the cell style
type: docs
url: /net/aspose.cells/cell/setstyle/
---
## SetStyle(Style) {#setstyle}

Sets the cell style.

```csharp
public void SetStyle(Style style)
```

| Parameter | Type | Description |
| --- | --- | --- |
| style | Style | The cell style. |

### Remarks

If the border settings are changed, the border of adjust cells will be updated too.

### Examples

```csharp
// Called: cells[1048575, 16383].SetStyle(style);
[Test]
        public void Method_Style_()
        {
            caseName = "testClearFormats_Excel2007_001";
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            Style style = GetStyle(workbook);
            cells[0, 0].SetStyle(style);
            cells[0, 16383].SetStyle(style);
            cells[1048575, 0].SetStyle(style);
            cells[1048575, 16383].SetStyle(style);

            cells.ClearFormats(0, 0, 1048575, 16383);

            checkClearFormats_Excel2007_001(workbook);
            workbook.Save(Constants.destPath + "testClearFormats.xlsx");
            workbook = new Workbook(Constants.destPath + "testClearFormats.xlsx");
            checkClearFormats_Excel2007_001(workbook);
            workbook.Save(Constants.destPath + "testClearFormats.xml", SaveFormat.SpreadsheetML);
            workbook = new Workbook(Constants.destPath + "testClearFormats.xml");
            workbook.Save(Constants.destPath + "testClearFormats.xls");            
        }
```

### See Also

* class [Style](../../style/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetStyle(Style, bool) {#setstyle_2}

Apply the changed property of style to the cell.

```csharp
public void SetStyle(Style style, bool explicitFlag)
```

| Parameter | Type | Description |
| --- | --- | --- |
| style | Style | The cell style. |
| explicitFlag | Boolean | True, only overwriting formatting which is explicitly set. |

### Examples

```csharp
// Called: cell.SetStyle(cellStyle, true);
[Test]
        public void Method_Boolean_()
        {
            
            Workbook workbook = new Workbook();
            Aspose.Cells.Style cellStyle = workbook.CreateStyle();
            cellStyle.IsTextWrapped = true;
            cellStyle.VerticalAlignment = TextAlignmentType.Top;
            Cell cell = workbook.Worksheets[0].Cells["A1"];
            cell.SetStyle(cellStyle, true);
            Assert.AreEqual(cell.GetStyle().VerticalAlignment, TextAlignmentType.Top);

        }
```

### See Also

* class [Style](../../style/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetStyle(Style, StyleFlag) {#setstyle_1}

Apply the cell style based on flags.

```csharp
public void SetStyle(Style style, StyleFlag flag)
```

| Parameter | Type | Description |
| --- | --- | --- |
| style | Style | The cell style. |
| flag | StyleFlag | The style flag. |

### Examples

```csharp
// Called: cell.SetStyle(style, styleFlag);
[Test]
        public void Method_StyleFlag_()
        {

            var workbook = new Workbook(Constants.sourcePath + @"CellsNet47431.xlsx");
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
            workbook.Save(Constants.destPath + @"CellsNet47431.xlsx");
        }
```

### See Also

* class [Style](../../style/)
* class [StyleFlag](../../styleflag/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



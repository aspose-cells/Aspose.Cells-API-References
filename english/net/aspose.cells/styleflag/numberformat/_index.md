---
title: StyleFlag.NumberFormat
second_title: Aspose.Cells for .NET API Reference
description: StyleFlag property. Number format setting will be applied
type: docs
url: /net/aspose.cells/styleflag/numberformat/
---
## StyleFlag.NumberFormat property

Number format setting will be applied.

```csharp
public bool NumberFormat { get; set; }
```

### Examples

```csharp
// Called: styleFlag.NumberFormat = true; // only number format should be changed
[Test]
        public void Property_NumberFormat()
        {

            var workbook = new Workbook(Constants.sourcePath + @&quot;CellsNet47431.xlsx&quot;);
            var fromRange = workbook.Worksheets[0].Cells.CreateRange(1, 0, 5, 1).EntireRow; // copy rows 1 - 10
            var toRange = workbook.Worksheets[1].Cells.CreateRange(11, 0, 1, 1);

            toRange.Copy(fromRange); // copy the data from the range
            int iLastRow = fromRange.FirstRow + fromRange.RowCount;
            int iLastCol = fromRange.FirstColumn + fromRange.ColumnCount;
            for (int iRow = fromRange.FirstRow; iRow &lt; iLastRow; iRow++)
            {
                for (int iCol = fromRange.FirstColumn; iCol &lt; iLastCol; iCol++)
                {
                    Cell cell = workbook.Worksheets[0].Cells[iRow, iCol];
                    var style = cell.GetStyle(false);
                    style.Custom = &quot;0.000&quot;;

                    var styleFlag = new StyleFlag();
                    styleFlag.NumberFormat = true; // only number format should be changed
                    cell.SetStyle(style, styleFlag);

                    Assert.AreEqual(cell.GetStyle(false).Borders[BorderType.TopBorder].LineStyle, CellBorderType.None);
                }

            }
            toRange.Copy(fromRange); // copy the data from the range
            workbook.Save(Constants.destPath + @&quot;CellsNet47431.xlsx&quot;);
        }
```

### See Also

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



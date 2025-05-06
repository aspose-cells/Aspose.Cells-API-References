---
title: Cells.SetColumnWidth
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Sets the width of the specified column in normal view
type: docs
url: /net/aspose.cells/cells/setcolumnwidth/
---
## Cells.SetColumnWidth method

Sets the width of the specified column in normal view.

```csharp
public void SetColumnWidth(int column, double width)
```

| Parameter | Type | Description |
| --- | --- | --- |
| column | Int32 | Column index. |
| width | Double | Width of column.Column width must be between 0 and 255. |

### Remarks

To hide a column, sets column width to zero.

### Examples

```csharp
// Called: worksheet.Cells.SetColumnWidth(0, 10);
[Test]
        public void Method_Double_()
        {
            Workbook wb = new Workbook();

            // When you create a new workbook, a default &quot;Sheet1&quot; is added to the workbook.
            Worksheet worksheet = wb.Worksheets[0];

            //rows
            // Setting the height of the 4th row to 30 &amp; color
            worksheet.Cells.SetRowHeight(3, 30);
            var style = wb.CreateStyle();
            style.ForegroundColor = Color.PaleGreen;
            style.Pattern = BackgroundType.Solid;
            //Create style flag
            StyleFlag flag = new StyleFlag();
            flag.CellShading = true;
            worksheet.Cells.Rows[3].ApplyStyle(style, flag);

            // Hiding the 3rd row of the worksheet
            worksheet.Cells.HideRow(2);
            var style0 = wb.CreateStyle();
            style0.ForegroundColor = Color.Yellow;
            style0.Pattern = BackgroundType.Solid;
            //Create style flag
            StyleFlag flag0 = new StyleFlag();
            flag0.CellShading = true;
            worksheet.Cells.Rows[2].ApplyStyle(style0, flag0);

            //columns
            worksheet.Cells.SetColumnWidth(0, 10);
            var style1 = worksheet.Cells[&quot;A1&quot;].GetStyle();
            style1.ForegroundColor = Color.Red;
            style1.Pattern = BackgroundType.Solid;
            worksheet.Cells[&quot;A1&quot;].SetStyle(style1);

            worksheet.Cells.SetColumnWidth(1, 40);
            var style2 = worksheet.Cells[&quot;B1&quot;].GetStyle();
            style2.ForegroundColor = Color.Black;
            style2.Pattern = BackgroundType.Solid;
            worksheet.Cells[&quot;B1&quot;].SetStyle(style2);

            worksheet.Cells.SetColumnWidth(2, 5);
            var style3 = wb.CreateStyle();
            style3.ForegroundColor = Color.Yellow;
            style3.Pattern = BackgroundType.Solid;
            //Create style flag
            StyleFlag flag3 = new StyleFlag();
            flag3.CellShading = true;
            worksheet.Cells.Columns[2].ApplyStyle(style3, flag3);

            worksheet.Cells.SetColumnWidth(3, 30);
            var style4 = worksheet.Cells[&quot;D1&quot;].GetStyle();
            style4.ForegroundColor = Color.Blue;
            style4.Pattern = BackgroundType.Solid;
            worksheet.Cells[&quot;D1&quot;].SetStyle(style4);

            worksheet.Cells.SetColumnWidth(4, 10);
            var style5 = worksheet.Cells[&quot;E1&quot;].GetStyle();
            style5.ForegroundColor = Color.Green;
            style5.Pattern = BackgroundType.Solid;
            worksheet.Cells[&quot;E1&quot;].SetStyle(style5);

            // Hiding the 3rd column of the worksheet
            worksheet.Cells.HideColumn(2);
            wb.Save(Constants.destPath + &quot;CELLSNET46971.xlsx&quot;);
        }
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



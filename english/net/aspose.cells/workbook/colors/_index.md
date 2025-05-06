---
title: Workbook.Colors
second_title: Aspose.Cells for .NET API Reference
description: Workbook property. Returns colors in the palette for the spreadsheet
type: docs
url: /net/aspose.cells/workbook/colors/
---
## Workbook.Colors property

Returns colors in the palette for the spreadsheet.

```csharp
public Color[] Colors { get; }
```

### Remarks

The palette has 56 entries, each represented by an RGB value.

### Examples

```csharp
// Called: System.Drawing.Color iColorBRD = oWorkbook.Colors[14];
[Test]
        public void Property_Colors()
        {
            Workbook oWorkbook = new Workbook();
            Worksheet oWorksheet = oWorkbook.Worksheets[0];

            System.Drawing.Color iColorBGR = oWorkbook.Colors[18];
            System.Drawing.Color iColorBRD = oWorkbook.Colors[14];


            Style oStyleBRD = oWorkbook.CreateStyle();
            Aspose.Cells.StyleFlag oStyleFlagBRD = new Aspose.Cells.StyleFlag();

            oStyleBRD.Name = &quot;BRD&quot;;
            oStyleBRD.Borders.SetColor(System.Drawing.Color.Red);
            oStyleBRD.Borders.SetStyle(Aspose.Cells.CellBorderType.Thin);

            oStyleFlagBRD.TopBorder = true;
            oStyleFlagBRD.RightBorder = true;
            oStyleFlagBRD.BottomBorder = true;
            oStyleFlagBRD.LeftBorder = true;



            Aspose.Cells.Style oStyleBGR = oWorkbook.CreateStyle();
            Aspose.Cells.StyleFlag oStyleFlagBGR = new Aspose.Cells.StyleFlag();

            oStyleBGR.Name = &quot;BGR&quot;;
            oStyleBGR.ForegroundColor = iColorBGR;
            oStyleBGR.Pattern = Aspose.Cells.BackgroundType.Solid;

            oStyleFlagBGR.CellShading = true;



            int iRow = 0;
            Aspose.Cells.Range oRange = null;
            Aspose.Cells.Row oRow = null;
            int iColumn = 0;
            Aspose.Cells.Column oColumn = null;

            for (iColumn = 0; iColumn &lt;= 9; iColumn++)
            {
                oColumn = oWorksheet.Cells.Columns[iColumn];
                oColumn.ApplyStyle(oStyleBRD, oStyleFlagBRD);
            }



            oRange = oWorksheet.Cells.CreateRange(0, 0, 3, 5);
            oRange.ApplyStyle(oStyleBGR, oStyleFlagBGR);



            oRow = oWorksheet.Cells.Rows[4];
            oRow.ApplyStyle(oStyleBGR, oStyleFlagBGR);

            for (iRow = 6; iRow &lt;= 8; iRow++)
            {
                oRow = oWorksheet.Cells.Rows[iRow];
                oRow.ApplyStyle(oStyleBGR, oStyleFlagBGR);
            }



            oWorkbook.Save(Constants.destPath + &quot;ApplyStyle_128425.xls&quot;);
            oWorkbook = new Workbook(Constants.destPath + &quot;ApplyStyle_128425.xls&quot;);
            Cells cells = oWorkbook.Worksheets[0].Cells;
          

            Assert.AreEqual(cells[&quot;B8&quot;].GetStyle().Borders[BorderType.TopBorder].Color.ToArgb() &amp; 0xFFFFFF,
               System.Drawing.Color.Red.ToArgb() &amp; 0xFFFFFF);
            Assert.AreEqual(cells[&quot;B9&quot;].GetStyle().Borders[BorderType.TopBorder].Color.ToArgb() &amp; 0xFFFFFF,
               System.Drawing.Color.Red.ToArgb() &amp; 0xFFFFFF);
        }
```

### See Also

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



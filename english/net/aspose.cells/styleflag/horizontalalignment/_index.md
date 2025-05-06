---
title: StyleFlag.HorizontalAlignment
second_title: Aspose.Cells for .NET API Reference
description: StyleFlag property. Horizontal alignment setting will be applied
type: docs
url: /net/aspose.cells/styleflag/horizontalalignment/
---
## StyleFlag.HorizontalAlignment property

Horizontal alignment setting will be applied.

```csharp
public bool HorizontalAlignment { get; set; }
```

### Examples

```csharp
// Called: flagDataRange.HorizontalAlignment = true;
[Test]
        public void Property_HorizontalAlignment()
        {
            Workbook workbook = new Workbook();
            Color color = Color.FromArgb(255, 250, 223);
            workbook.ChangePalette(color, 55);
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            int rows = 10000;
            int numberOfColumns = 200;
            //Fill Data in 10000 * 200 matrix.
            for (int i = 0; i &lt;= rows; i++)
            {
                for (int j = 0; j &lt;= numberOfColumns; j++)
                {

                    cells[i, j].PutValue(i.ToString() + &quot;,&quot; + j.ToString());
                }
            }

            //Apply to range style.
            Aspose.Cells.Range objRangeData = worksheet.Cells.CreateRange(0, 0, 1000, 50);
            objRangeData.Name = &quot;DataRange&quot;;
            Aspose.Cells.Style StyleDataRange = workbook.CreateStyle();
            StyleDataRange.Font.Name = &quot;Arial&quot;;
            StyleDataRange.Font.Size = 8;
            StyleDataRange.Font.Color = System.Drawing.Color.Black;
            StyleDataRange.HorizontalAlignment = TextAlignmentType.Left;
            StyleDataRange.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thin;
            StyleDataRange.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Thin;
            StyleDataRange.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Thin;
            StyleDataRange.Borders[BorderType.LeftBorder].LineStyle = CellBorderType.Thin;
            StyleDataRange.ForegroundColor = System.Drawing.Color.FromArgb(255, 250, 223);
            StyleDataRange.Pattern = BackgroundType.Solid;

            //Define a style flag struct.
            StyleFlag flagDataRange = new StyleFlag();
            flagDataRange.CellShading = true;
            flagDataRange.FontName = true;
            flagDataRange.FontSize = true;
            flagDataRange.FontColor = true;
            flagDataRange.HorizontalAlignment = true;
            flagDataRange.Borders = true;
            flagDataRange.ShrinkToFit = true;
            flagDataRange.WrapText = true;

            objRangeData.ApplyStyle(StyleDataRange, flagDataRange);
            SpreadsheetML2003SaveOptions saveOptions = new SpreadsheetML2003SaveOptions(SaveFormat.Csv);
            saveOptions.CachedFileFolder = Constants.destPath;
            workbook.Save(Constants.destPath + &quot;testSave.CSV&quot;, saveOptions);
        }
```

### See Also

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



---
title: StyleFlag.Borders
second_title: Aspose.Cells for .NET API Reference
description: StyleFlag property. All borders settings will be applied
type: docs
url: /net/aspose.cells/styleflag/borders/
---
## StyleFlag.Borders property

All borders settings will be applied.

```csharp
public bool Borders { get; set; }
```

### Examples

```csharp
// Called: styleFlagGrid.Borders = true;
protected static void Property_Borders(Workbook book)
        {
            StyleFlag styleFlagGrid = new StyleFlag();
            styleFlagGrid.Borders = true;
            for (int i = 0; i &lt; book.Worksheets.Count; i++)
            {
                Worksheet sheet = book.Worksheets[i];
                int maxRow = sheet.Cells.MaxRow;
                int maxCol = sheet.Cells.MaxColumn;
                for (int datai = 0; datai &lt;= maxRow; datai++)
                {
                    for (int datay = 0; datay &lt;= maxCol; datay++)
                    {
                        Cell dataCell = sheet.Cells[datai, datay];
                        Style dataStyle = dataCell.GetStyle();
                        if (dataStyle.Borders[BorderType.LeftBorder].LineStyle == 0)
                        {
                            dataStyle.SetBorder(BorderType.LeftBorder, CellBorderType.Thin, System.Drawing.Color.FromArgb(255, 204, 204, 204));
                        }
                        if (dataStyle.Borders[BorderType.RightBorder].LineStyle == 0)
                        {
                            dataStyle.SetBorder(BorderType.RightBorder, CellBorderType.Thin, System.Drawing.Color.FromArgb(255, 204, 204, 204));
                        }
                        if (dataStyle.Borders[BorderType.BottomBorder].LineStyle == 0)
                        {
                            dataStyle.SetBorder(BorderType.BottomBorder, CellBorderType.Thin, System.Drawing.Color.FromArgb(255, 204, 204, 204));
                        }
                        if (dataStyle.Borders[BorderType.TopBorder].LineStyle == 0)
                        {
                            dataStyle.SetBorder(BorderType.TopBorder, CellBorderType.Thin, System.Drawing.Color.FromArgb(255, 204, 204, 204));
                        }
                        dataCell.SetStyle(dataStyle, styleFlagGrid);

                        dataCell.GetStyle().Number = 49;
                    }
                }
            }
        }
```

### See Also

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



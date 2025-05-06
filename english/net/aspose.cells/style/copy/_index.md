---
title: Style.Copy
second_title: Aspose.Cells for .NET API Reference
description: Style method. Copies data from another style object
type: docs
url: /net/aspose.cells/style/copy/
---
## Style.Copy method

Copies data from another style object

```csharp
public void Copy(Style style)
```

| Parameter | Type | Description |
| --- | --- | --- |
| style | Style | Source Style object |

### Remarks

This method does not copy the name of the style. If you want to copy the name, please call the following codes after copying style: destStyle.Name = style.Name.

### Examples

```csharp
// Called: style2.Copy(style1);
public void Method_Style_(Workbook workbook)
        {
            Style style1 = workbook.CreateStyle();

            //Set borders
            style1.Borders[BorderType.TopBorder].Color = Color.FromArgb(0, 0, 128);
            style1.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thin;
            style1.Borders[BorderType.BottomBorder].Color = Color.FromArgb(0, 0, 128);
            style1.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Thin;
            style1.Borders[BorderType.LeftBorder].Color = Color.FromArgb(0, 0, 128);
            style1.Borders[BorderType.LeftBorder].LineStyle = CellBorderType.Thin;
            style1.Borders[BorderType.RightBorder].Color = Color.FromArgb(0, 0, 128);
            style1.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Thin;
            style1.Font.IsBold = true;
            style1.HorizontalAlignment = TextAlignmentType.Center;

            Cells cells = workbook.Worksheets[0].Cells;
            //Set the width of the specified column 
            cells.SetColumnWidth(0, 12);
            cells.SetColumnWidth(1, 10);

            cells[&quot;A1&quot;].SetStyle(style1);
            cells[&quot;B1&quot;].SetStyle(style1);

            Style style2 = workbook.CreateStyle();
            //Copy data from another style object
            style2.Copy(style1);
            style2.Font.IsBold = false;
            //Set foreground color
            style2.ForegroundColor = Color.FromArgb(255, 255, 204);
            style2.Pattern = BackgroundType.Solid;
            style2.HorizontalAlignment = TextAlignmentType.Right;

            for (int i = 1; i &lt;= 9; i++)
            {
                if (i % 2 != 0)
                {
                    cells[i, 0].SetStyle(style2);
                    cells[i, 1].SetStyle(style2);
                }
            }

            Style style3 = workbook.CreateStyle();
            style3.Copy(style2);
            //Set foreground color
            style3.ForegroundColor = Color.FromArgb(204, 255, 204);
            style3.Pattern = BackgroundType.Solid;

            for (int j = 1; j &lt;= 9; j++)
            {
                if (j % 2 == 0)
                {
                    cells[j, 0].SetStyle(style3);
                    cells[j, 1].SetStyle(style3);
                }
            }
        }
```

### See Also

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



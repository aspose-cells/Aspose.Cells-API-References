---
title: Cells.SetViewColumnWidthPixel
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Sets the width of the column in different view
type: docs
url: /net/aspose.cells/cells/setviewcolumnwidthpixel/
---
## Cells.SetViewColumnWidthPixel method

Sets the width of the column in different view.

```csharp
public void SetViewColumnWidthPixel(int column, int pixels)
```

| Parameter | Type | Description |
| --- | --- | --- |
| column | Int32 | The column index. |
| pixels | Int32 | The width in unit of pixels. |

### Remarks

If the current view type is PageLayoutView, the column's width is same as printed width.

### Examples

```csharp
// Called: sheet.Cells.SetViewColumnWidthPixel(1, intPixels);
public void Cells_Method_SetViewColumnWidthPixel()
{
    Workbook wb = new Workbook(Constants.sourcePath + "example.xltx");

    Worksheet sheet = wb.Worksheets[0];

    sheet.Cells[1, 1].Value = "19:00 Schneekönigin";

    // sheet.Cells[1, 2].Value = "cell to the right";
    sheet.Cells[2, 1].Value = "cell below ";

    Style style = sheet.Cells[1, 1].GetStyle();
    //style.SetBorder(BorderType.LeftBorder | BorderType.RightBorder | BorderType.BottomBorder, CellBorderType.Thin, Color.Black);
    style.IsTextWrapped = true;
    sheet.Cells[1, 1].SetStyle(style);

    sheet.ViewType = ViewType.PageLayoutView;
    //30mm 
    double dblWidthInch = (30 / 10) * 0.39370;
    //Mit dem DPI-Faktor multiplizieren.
    int intPixels = (int)(dblWidthInch * 96);
    sheet.Cells.SetViewColumnWidthPixel(1, intPixels);
    sheet.ViewType = ViewType.NormalView;

    AutoFitterOptions afo = new AutoFitterOptions();
    afo.AutoFitMergedCellsType = AutoFitMergedCellsType.LastLine;
    //If this line is removed, the cell has a different height:
    sheet.AutoFitRows(1, 1, afo);
    Assert.IsTrue(sheet.Cells.Rows[1].IsHeightMatched);
    wb.Save(Constants.destPath + "example.xlsx");
}
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



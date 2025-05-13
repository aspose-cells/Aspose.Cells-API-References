---
title: StyleFlag.RightBorder
second_title: Aspose.Cells for .NET API Reference
description: StyleFlag property. Right border settings will be applied
type: docs
url: /net/aspose.cells/styleflag/rightborder/
---
## StyleFlag.RightBorder property

Right border settings will be applied.

```csharp
public bool RightBorder { get; set; }
```

### Examples

```csharp
// Called: oStyleFlagBRD.RightBorder = true;
public void StyleFlag_Property_RightBorder()
{
    Workbook oWorkbook = new Workbook();
    Worksheet oWorksheet = oWorkbook.Worksheets[0];

    System.Drawing.Color iColorBGR = oWorkbook.Colors[18];
    System.Drawing.Color iColorBRD = oWorkbook.Colors[14];


    Style oStyleBRD = oWorkbook.CreateStyle();
    Aspose.Cells.StyleFlag oStyleFlagBRD = new Aspose.Cells.StyleFlag();

    oStyleBRD.Name = "BRD";
    oStyleBRD.Borders.SetColor(System.Drawing.Color.Red);
    oStyleBRD.Borders.SetStyle(Aspose.Cells.CellBorderType.Thin);

    oStyleFlagBRD.TopBorder = true;
    oStyleFlagBRD.RightBorder = true;
    oStyleFlagBRD.BottomBorder = true;
    oStyleFlagBRD.LeftBorder = true;



    Aspose.Cells.Style oStyleBGR = oWorkbook.CreateStyle();
    Aspose.Cells.StyleFlag oStyleFlagBGR = new Aspose.Cells.StyleFlag();

    oStyleBGR.Name = "BGR";
    oStyleBGR.ForegroundColor = iColorBGR;
    oStyleBGR.Pattern = Aspose.Cells.BackgroundType.Solid;

    oStyleFlagBGR.CellShading = true;



    int iRow = 0;
    Aspose.Cells.Range oRange = null;
    Aspose.Cells.Row oRow = null;
    int iColumn = 0;
    Aspose.Cells.Column oColumn = null;

    for (iColumn = 0; iColumn <= 9; iColumn++)
    {
        oColumn = oWorksheet.Cells.Columns[iColumn];
        oColumn.ApplyStyle(oStyleBRD, oStyleFlagBRD);
    }



    oRange = oWorksheet.Cells.CreateRange(0, 0, 3, 5);
    oRange.ApplyStyle(oStyleBGR, oStyleFlagBGR);



    oRow = oWorksheet.Cells.Rows[4];
    oRow.ApplyStyle(oStyleBGR, oStyleFlagBGR);

    for (iRow = 6; iRow <= 8; iRow++)
    {
        oRow = oWorksheet.Cells.Rows[iRow];
        oRow.ApplyStyle(oStyleBGR, oStyleFlagBGR);
    }



    oWorkbook.Save(Constants.destPath + "example.xls");
    oWorkbook = new Workbook(Constants.destPath + "example.xls");
    Cells cells = oWorkbook.Worksheets[0].Cells;
          

    Assert.AreEqual(cells["B8"].GetStyle().Borders[BorderType.TopBorder].Color.ToArgb() & 0xFFFFFF,
       System.Drawing.Color.Red.ToArgb() & 0xFFFFFF);
    Assert.AreEqual(cells["B9"].GetStyle().Borders[BorderType.TopBorder].Color.ToArgb() & 0xFFFFFF,
       System.Drawing.Color.Red.ToArgb() & 0xFFFFFF);
}
```

### See Also

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



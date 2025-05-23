---
title: Cells.GetRowHeightInch
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Gets the height of a specified row in unit of inches
type: docs
url: /net/aspose.cells/cells/getrowheightinch/
---
## Cells.GetRowHeightInch method

Gets the height of a specified row in unit of inches.

```csharp
public double GetRowHeightInch(int row)
```

| Parameter | Type | Description |
| --- | --- | --- |
| row | Int32 | Row index |

### Return Value

Height of row

### Examples

```csharp
// Called: Assert.AreEqual(2, cells2.GetRowHeightInch(j), 0.01);
public void Cells_Method_GetRowHeightInch()
{
    //==============Write==================//
    Workbook workbook1 = new Workbook();
    Style defaultstyle = workbook1.DefaultStyle;
    defaultstyle.Font.Name = "Tahoma";
    defaultstyle.Font.Size = 16;
    defaultstyle.Font.IsBold = true;
    workbook1.DefaultStyle = defaultstyle;

    Cells cells1= workbook1.Worksheets[0].Cells;
    cells1.SetColumnWidthInch(0, 2);
    cells1.SetColumnWidthInch(1, 2.1);
    int i;
    // Column widths
    for (i = 2; i < 13; i++)
    {
        cells1.SetColumnWidthInch(i, 1.2);
    }
    cells1.SetColumnWidthInch(i, 1);
    cells1.SetColumnWidthInch(i + 1, 2);
    //Row heights
    cells1.SetRowHeightInch(i, 2);
    for (i = 37; i < 128; i++)
        cells1.SetRowHeightInch(i, 5.6875);
    workbook1.Save(Constants.destPath + "SetRowHeightInch.xls");
    //==================Read==================//
    Workbook workbook2 = new Workbook(Constants.destPath + "SetRowHeightInch.xls");
    Cells cells2 = workbook2.Worksheets[0].Cells;
    Assert.AreEqual(2, cells2.GetColumnWidth(0, false, CellsUnitType.Inch), 0.01);
    //Assert.AreEqual(2.1, cells2.GetColumnWidthInch(1), 0.0001);
    int j;
    // Column widths
    for (j = 2; j < 13; j++)
    {
        Assert.AreEqual(1.2, cells2.GetColumnWidth(j, false, CellsUnitType.Inch), 0.01);
    }
    Assert.AreEqual(1, cells2.GetColumnWidth(j, false, CellsUnitType.Inch), 0.01);
    Assert.AreEqual(2, cells2.GetColumnWidth(j + 1, false, CellsUnitType.Inch), 0.01);
    //Rows heights
    Assert.AreEqual(2, cells2.GetRowHeightInch(j), 0.01);
    for (j = 37; j < 128; j++)
    {
        Assert.AreEqual(5.6875, cells2.GetRowHeightInch(j), 0.01);
    }
}
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



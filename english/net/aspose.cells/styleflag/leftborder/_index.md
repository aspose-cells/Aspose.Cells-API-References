---
title: StyleFlag.LeftBorder
second_title: Aspose.Cells for .NET API Reference
description: StyleFlag property. Left border settings will be applied
type: docs
url: /net/aspose.cells/styleflag/leftborder/
---
## StyleFlag.LeftBorder property

Left border settings will be applied.

```csharp
public bool LeftBorder { get; set; }
```

### Examples

```csharp
// Called: flag.LeftBorder = true;
public void StyleFlag_Property_LeftBorder()
{
    var workbook = new Workbook();
    workbook.Settings.UpdateAdjacentCellsBorder = true;
    var worksheet = workbook.Worksheets[0];

    var range = worksheet.Cells.CreateRange(1, 1, 6, 6);
    var style = worksheet.Workbook.CreateStyle();
    var flag = new StyleFlag();

    ApplyColorBorder(style, BorderType.BottomBorder, "blue");
    ApplyStyleBorder(style, BorderType.BottomBorder, CellBorderType.Thick);
    flag.BottomBorder = true;

    ApplyColorBorder(style, BorderType.LeftBorder, "blue");
    ApplyStyleBorder(style, BorderType.LeftBorder, CellBorderType.Thick);
    flag.LeftBorder = true;

    ApplyColorBorder(style, BorderType.RightBorder, "blue");
    ApplyStyleBorder(style, BorderType.RightBorder, CellBorderType.Thick);
    flag.RightBorder = true;

    ApplyColorBorder(style, BorderType.TopBorder, "blue");
    ApplyStyleBorder(style, BorderType.TopBorder, CellBorderType.Thick);
    flag.TopBorder = true;
    range.ApplyStyle(style, flag);
    //everything should be blue at this moment

    //set left border DOESNT WORK
    range = worksheet.Cells.CreateRange(2, 2, 1, 1);
    range.PutValue("left border", false, false);
    style = worksheet.Workbook.CreateStyle();
    flag = new StyleFlag();
    ApplyColorBorder(style, BorderType.LeftBorder, "green");
    ApplyStyleBorder(style, BorderType.LeftBorder, CellBorderType.Thick);
    flag.LeftBorder = true;
    range.ApplyStyle(style, flag);
   AssertHelper.AreEqual(worksheet.Cells[2,2].GetStyle().Borders[BorderType.LeftBorder].Color, Color.Green);

    //set right border DOESNT WORK
    range = worksheet.Cells.CreateRange(2, 3, 1, 1);
    range.PutValue("right orange", false, false);
    style = worksheet.Workbook.CreateStyle();
    flag = new StyleFlag();
    ApplyColorBorder(style, BorderType.RightBorder, "orange");
    ApplyStyleBorder(style, BorderType.RightBorder, CellBorderType.Thick);
    flag.RightBorder = true;
    range.ApplyStyle(style, flag);
   AssertHelper.AreEqual(worksheet.Cells[2, 3].GetStyle().Borders[BorderType.RightBorder].Color, Color.Orange);


    //set top border DOESNT WORK
    range = worksheet.Cells.CreateRange(3, 2, 1, 1);
    range.PutValue("top pink ", false, false);
    style = worksheet.Workbook.CreateStyle();
    flag = new StyleFlag();
    ApplyColorBorder(style, BorderType.TopBorder, "pink");
    ApplyStyleBorder(style, BorderType.TopBorder, CellBorderType.Thick);
    flag.TopBorder = true;
    range.ApplyStyle(style, flag);
   AssertHelper.AreEqual(worksheet.Cells[3, 2].GetStyle().Borders[BorderType.TopBorder].Color, Color.Pink);


    //set left border DOESNT WORK
    range = worksheet.Cells.CreateRange(3, 3, 1, 1);
    range.PutValue("bottom brown", false, false);
    style = worksheet.Workbook.CreateStyle();
    flag = new StyleFlag();
    ApplyColorBorder(style, BorderType.BottomBorder, "brown");
    ApplyStyleBorder(style, BorderType.BottomBorder, CellBorderType.Thick);
    flag.BottomBorder = true;
    range.ApplyStyle(style, flag);
   AssertHelper.AreEqual(worksheet.Cells[3, 3].GetStyle().Borders[BorderType.BottomBorder].Color, Color.Brown);


    //set left border WORKS only when it's on the last row
    range = worksheet.Cells.CreateRange(6, 1, 1, 1);
    range.PutValue("left border", false, false);
    style = worksheet.Workbook.CreateStyle();
    flag = new StyleFlag();
    ApplyColorBorder(style, BorderType.LeftBorder, "green");
    ApplyStyleBorder(style, BorderType.LeftBorder, CellBorderType.Thick);
    flag.LeftBorder = true;
    range.ApplyStyle(style, flag);
   AssertHelper.AreEqual(worksheet.Cells[6, 1].GetStyle().Borders[BorderType.LeftBorder].Color, Color.Green);


    //set right border DOESNT WORK
    range = worksheet.Cells.CreateRange(6, 2, 1, 1);
    range.PutValue("right orange", false, false);
    style = worksheet.Workbook.CreateStyle();
    flag = new StyleFlag();
    ApplyColorBorder(style, BorderType.RightBorder, "orange");
    ApplyStyleBorder(style, BorderType.RightBorder, CellBorderType.Thick);
    flag.RightBorder = true;
    range.ApplyStyle(style, flag);
   AssertHelper.AreEqual(worksheet.Cells[6, 2].GetStyle().Borders[BorderType.RightBorder].Color, Color.Orange);


    //set top border DOESNT WORK
    range = worksheet.Cells.CreateRange(6, 3, 1, 1);
    range.PutValue("top pink ", false, false);
    style = worksheet.Workbook.CreateStyle();
    flag = new StyleFlag();
    ApplyColorBorder(style, BorderType.TopBorder, "pink");
    ApplyStyleBorder(style, BorderType.TopBorder, CellBorderType.Thick);
    flag.TopBorder = true;
    range.ApplyStyle(style, flag);
   AssertHelper.AreEqual(worksheet.Cells[6, 3].GetStyle().Borders[BorderType.TopBorder].Color, Color.Pink);


    //set bottom border WORK only when it's on the last row
    range = worksheet.Cells.CreateRange(6, 4, 1, 1);
    range.PutValue("bottom brown", false, false);
    style = worksheet.Workbook.CreateStyle();
    flag = new StyleFlag();
    ApplyColorBorder(style, BorderType.BottomBorder, "brown");
    ApplyStyleBorder(style, BorderType.BottomBorder, CellBorderType.Thick);
    flag.BottomBorder = true;
    range.ApplyStyle(style, flag);
   AssertHelper.AreEqual(worksheet.Cells[6, 4].GetStyle().Borders[BorderType.BottomBorder].Color, Color.Brown);


    worksheet.AutoFitColumns(1, 1, 6, 6);
    workbook.Save(Constants.destPath + "example.xlsx");
}
```

### See Also

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



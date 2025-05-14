---
title: Style.HorizontalAlignment
second_title: Aspose.Cells for .NET API Reference
description: Style property. Gets or sets the horizontal alignment type of the text in a cell
type: docs
url: /net/aspose.cells/style/horizontalalignment/
---
## Style.HorizontalAlignment property

Gets or sets the horizontal alignment type of the text in a cell.

```csharp
public TextAlignmentType HorizontalAlignment { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(cells["A1"].GetStyle().HorizontalAlignment, TextAlignmentType.Left);
public void Style_Property_HorizontalAlignment()
{
    string filePath = Constants.JohnTest_PATH_SOURCE + @"JAVA42110AndNET45000/";
    Workbook wb = new Workbook(filePath + "a.html");
    Cells cells = wb.Worksheets[0].Cells;
    Assert.AreEqual(cells["A1"].GetStyle().HorizontalAlignment, TextAlignmentType.Left);
    Assert.AreEqual(cells["A1"].GetStyle().Font.Color, Color.FromArgb(255, 255, 0, 0));

    Assert.AreEqual(cells["A2"].GetStyle().HorizontalAlignment, TextAlignmentType.Center);
    Assert.AreEqual(cells["A2"].GetStyle().Font.Color, Color.FromArgb(255, 0, 128, 0));
    wb.Save(CreateFolder(filePath) + "out.xlsx");
}
```

### See Also

* enum [TextAlignmentType](../../textalignmenttype/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



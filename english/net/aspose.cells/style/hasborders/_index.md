---
title: Style.HasBorders
second_title: Aspose.Cells for .NET API Reference
description: Style property. Checks whether there are borders have been set for the style
type: docs
url: /net/aspose.cells/style/hasborders/
---
## Style.HasBorders property

Checks whether there are borders have been set for the style.

```csharp
public bool HasBorders { get; }
```

### Examples

```csharp
// Called: Assert.IsFalse(cells["B9"].GetStyle().HasBorders);
public void Style_Property_HasBorders()
{
    Workbook workbook = new Workbook(Constants.HtmlPath + "example.html");
    workbook.Save(_destFilesPath + "example.xlsx");
    Cells cells = workbook.Worksheets[0].Cells;
    Assert.IsFalse(cells["A8"].GetStyle().HasBorders);
    Assert.IsFalse(cells["B9"].GetStyle().HasBorders);
    Assert.AreEqual(CellBorderType.Thin , cells["C8"].GetStyle().Borders[BorderType.TopBorder].LineStyle);
    Assert.AreEqual(TextAlignmentType.Left , cells["A10"].GetStyle().HorizontalAlignment);
    Assert.AreEqual(TextAlignmentType.Right , cells["C10"].GetStyle().HorizontalAlignment);
}
```

### See Also

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



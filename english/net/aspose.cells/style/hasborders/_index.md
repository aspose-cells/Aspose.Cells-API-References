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
// Called: Assert.IsFalse(cells[&amp;quot;A8&amp;quot;].GetStyle().HasBorders);
[Test]
        public void Property_HasBorders()
        {
            Workbook workbook = new Workbook(Constants.HtmlPath + &quot;CELLSNET-57107.html&quot;);
            workbook.Save(_destFilesPath + &quot;CELLSNET-57107.xlsx&quot;);
            Cells cells = workbook.Worksheets[0].Cells;
            Assert.IsFalse(cells[&quot;A8&quot;].GetStyle().HasBorders);
            Assert.IsFalse(cells[&quot;B9&quot;].GetStyle().HasBorders);
            Assert.AreEqual(CellBorderType.Thin , cells[&quot;C8&quot;].GetStyle().Borders[BorderType.TopBorder].LineStyle);
            Assert.AreEqual(TextAlignmentType.Left , cells[&quot;A10&quot;].GetStyle().HorizontalAlignment);
            Assert.AreEqual(TextAlignmentType.Right , cells[&quot;C10&quot;].GetStyle().HorizontalAlignment);
        }
```

### See Also

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



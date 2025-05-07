---
title: Style.VerticalAlignment
second_title: Aspose.Cells for .NET API Reference
description: Style property. Gets or sets the vertical alignment type of the text in a cell
type: docs
url: /net/aspose.cells/style/verticalalignment/
---
## Style.VerticalAlignment property

Gets or sets the vertical alignment type of the text in a cell.

```csharp
public TextAlignmentType VerticalAlignment { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(style.VerticalAlignment, TextAlignmentType.Bottom);
[Test]
        public void Property_VerticalAlignment()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CELLSNET-42087.xml");
            Style style = workbook.Worksheets[0].Cells["B7"].GetStyle();
            Assert.AreEqual(style.VerticalAlignment, TextAlignmentType.Bottom);
        }
```

### See Also

* enum [TextAlignmentType](../../textalignmenttype/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



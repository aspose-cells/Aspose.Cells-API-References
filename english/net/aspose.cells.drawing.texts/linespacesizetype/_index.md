---
title: Enum LineSpaceSizeType
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Drawing.Texts.LineSpaceSizeType enum. Represents the unit type of line space size
type: docs
url: /net/aspose.cells.drawing.texts/linespacesizetype/
---
## LineSpaceSizeType enumeration

Represents the unit type of line space size.

```csharp
public enum LineSpaceSizeType
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| Percentage | `0` | Represents in unit of a percentage of the text size. |
| Points | `1` | Represents in unit of points. |

### Examples

```csharp
// Called: Assert.AreEqual(p.SpaceAfterSizeType, LineSpaceSizeType.Points);
[Test]
        public void Type_LineSpaceSizeType()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CellsNet44866.xlsx&quot;);
            workbook.Save(Constants.destPath + &quot;CellsNet44866.xlsx&quot;);
            workbook = new Workbook(Constants.destPath + &quot;CellsNet44866.xlsx&quot;);
         ShapeCollection shapes = workbook.Worksheets[0].Charts[0].Shapes;
            foreach(Shape shape in shapes)
            {
                if (shape.Text !=null &amp;&amp; shape.Text.IndexOf(&quot;All com&quot;) != -1)
                {
                    TextParagraph p = (TextParagraph)shape.TextBody[0];
                    Assert.AreEqual(p.SpaceAfterSizeType, LineSpaceSizeType.Points);
                    break;
                }
            }

        }
```

### See Also

* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)



---
title: TextParagraph.SpaceAfterSizeType
second_title: Aspose.Cells for .NET API Reference
description: TextParagraph property. Gets and sets the amount of vertical white space that will be present after a paragraph
type: docs
url: /net/aspose.cells.drawing.texts/textparagraph/spaceaftersizetype/
---
## TextParagraph.SpaceAfterSizeType property

Gets and sets the amount of vertical white space that will be present after a paragraph.

```csharp
public LineSpaceSizeType SpaceAfterSizeType { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(p.SpaceAfterSizeType, LineSpaceSizeType.Points);
[Test]
        public void Property_SpaceAfterSizeType()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CellsNet44866.xlsx");
            workbook.Save(Constants.destPath + "CellsNet44866.xlsx");
            workbook = new Workbook(Constants.destPath + "CellsNet44866.xlsx");
         ShapeCollection shapes = workbook.Worksheets[0].Charts[0].Shapes;
            foreach(Shape shape in shapes)
            {
                if (shape.Text !=null && shape.Text.IndexOf("All com") != -1)
                {
                    TextParagraph p = (TextParagraph)shape.TextBody[0];
                    Assert.AreEqual(p.SpaceAfterSizeType, LineSpaceSizeType.Points);
                    break;
                }
            }

        }
```

### See Also

* enum [LineSpaceSizeType](../../linespacesizetype/)
* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)



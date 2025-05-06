---
title: FontSettingCollection.TextAlignment
second_title: Aspose.Cells for .NET API Reference
description: FontSettingCollection property. Represents the alignment setting of the text body
type: docs
url: /net/aspose.cells.drawing.texts/fontsettingcollection/textalignment/
---
## FontSettingCollection.TextAlignment property

Represents the alignment setting of the text body.

```csharp
public ShapeTextAlignment TextAlignment { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(72, shape.TextBody.TextAlignment.BottomMarginPt);
[Test]
        public void Property_TextAlignment()
        {
            var wb = new Workbook(Constants.sourcePath + &quot;CellsNet45886.xlsx&quot;);
            Shape shape = wb.Worksheets[0].Shapes[0];
            Assert.IsFalse(shape.TextBody.TextAlignment.IsAutoMargin);
            Assert.AreEqual(72, shape.TextBody.TextAlignment.BottomMarginPt);
            Assert.AreEqual(72, shape.TextBody.TextAlignment.TopMarginPt);
            Assert.AreEqual(72, shape.TextBody.TextAlignment.RightMarginPt);
            Assert.AreEqual(72, shape.TextBody.TextAlignment.BottomMarginPt);
            Assert.AreEqual(72, shape.TextBody.TextAlignment.LeftMarginPt);

            shape.TextBody.TextAlignment.BottomMarginPt = 36;
            shape.TextBody.TextAlignment.RightMarginPt = 18;
            shape.TextBody.TextAlignment.LeftMarginPt = 54;
            wb.Save(Constants.destPath + &quot;CellsNet45886.xlsx&quot;);
            wb = new Workbook(Constants.destPath + &quot;CellsNet45886.xlsx&quot;);
            Assert.AreEqual(36, shape.TextBody.TextAlignment.BottomMarginPt);
        }
```

### See Also

* class [ShapeTextAlignment](../../shapetextalignment/)
* class [FontSettingCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)



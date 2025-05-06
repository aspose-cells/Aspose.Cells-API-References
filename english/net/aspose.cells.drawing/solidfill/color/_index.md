---
title: SolidFill.Color
second_title: Aspose.Cells for .NET API Reference
description: SolidFill property. Gets or sets the Color
type: docs
url: /net/aspose.cells.drawing/solidfill/color/
---
## SolidFill.Color property

Gets or sets the Color.

```csharp
public Color Color { get; set; }
```

### Examples

```csharp
// Called: Assert.IsTrue(Util.CompareColor(Color.FromArgb(255, 255, 225), comment.CommentShape.Fill.SolidFill.Color));
[Test]
        public void Property_Color()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CELLSNET52822.xlsm&quot;);
            Workbook a = new Workbook();
            a.Worksheets[0].Copy(workbook.Worksheets[0]);        

            a.Save(Constants.destPath + &quot;CELLSNET52822.xlsx&quot;);
            Assert.IsTrue(a.Worksheets[0].Comments[0].CommentShape.TextBody.TextAlignment.IsAutoMargin);
            Comment comment = a.Worksheets[0].Comments[0];
            Assert.IsTrue(Util.CompareColor(Color.FromArgb(255, 255, 225), comment.CommentShape.Fill.SolidFill.Color));
            Assert.AreEqual(&quot;ＭＳ Ｐゴシック&quot;, comment.Font.Name);
            Assert.AreEqual(9, comment.Font.Size);

        }
```

### See Also

* class [SolidFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)



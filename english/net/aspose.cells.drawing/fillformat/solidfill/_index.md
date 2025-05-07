---
title: FillFormat.SolidFill
second_title: Aspose.Cells for .NET API Reference
description: FillFormat property. Gets SolidFill object
type: docs
url: /net/aspose.cells.drawing/fillformat/solidfill/
---
## FillFormat.SolidFill property

Gets `SolidFill` object.

```csharp
public SolidFill SolidFill { get; }
```

### Examples

```csharp
// Called: Assert.IsTrue(Util.CompareColor(Color.FromArgb(255, 255, 225), comment.CommentShape.Fill.SolidFill.Color));
[Test]
        public void Property_SolidFill()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CELLSNET52822.xlsm");
            Workbook a = new Workbook();
            a.Worksheets[0].Copy(workbook.Worksheets[0]);        

            a.Save(Constants.destPath + "CELLSNET52822.xlsx");
            Assert.IsTrue(a.Worksheets[0].Comments[0].CommentShape.TextBody.TextAlignment.IsAutoMargin);
            Comment comment = a.Worksheets[0].Comments[0];
            Assert.IsTrue(Util.CompareColor(Color.FromArgb(255, 255, 225), comment.CommentShape.Fill.SolidFill.Color));
            Assert.AreEqual("ＭＳ Ｐゴシック", comment.Font.Name);
            Assert.AreEqual(9, comment.Font.Size);

        }
```

### See Also

* class [SolidFill](../../solidfill/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)



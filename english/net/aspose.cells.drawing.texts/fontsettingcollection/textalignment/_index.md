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
// Called: workbook.Worksheets[0].Shapes[2].TextBody.TextAlignment.AutoSize = false;
[Test]
        // http://www.aspose.com/community/forums/thread/240759.aspx
        public void Property_TextAlignment()
        {
            Console.WriteLine("Property_TextAlignment()");
            string infn = path + "Test_CommentAutoSize.xlsx";
            string outfn = Constants.destPath + "Test_CommentAutoSize_out.xlsx";
            string outfn2 = Constants.destPath + "Test_CommentAutoSize_out_2.xlsx";

            Workbook workbook = new Workbook(infn);

            workbook.Worksheets[0].Comments[0].AutoSize = true;
            workbook.Worksheets[0].Shapes[2].TextBody.TextAlignment.AutoSize = true;

            workbook.Worksheets[0].Comments[workbook.Worksheets[0].Comments.Add("A1")].AutoSize = true;


            workbook.Save(outfn);

            workbook = new Workbook(outfn);

            workbook.Worksheets[0].Comments[0].AutoSize = false;
            workbook.Worksheets[0].Shapes[2].TextBody.TextAlignment.AutoSize = false;

            workbook.Save(outfn2);

        }
```

### See Also

* class [ShapeTextAlignment](../../shapetextalignment/)
* class [FontSettingCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)



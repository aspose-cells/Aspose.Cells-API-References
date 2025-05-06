---
title: MsoFormatPicture.TransparentColor
second_title: Aspose.Cells for .NET API Reference
description: MsoFormatPicture property. Gets and sets the transparent color of the picture
type: docs
url: /net/aspose.cells.drawing/msoformatpicture/transparentcolor/
---
## MsoFormatPicture.TransparentColor property

Gets and sets the transparent color of the picture.

```csharp
public CellsColor TransparentColor { get; set; }
```

### Examples

```csharp
// Called: CellsColor c = p.FormatPicture.TransparentColor;
[Test]
        // http://www.aspose.com/community/forums/thread/239329.aspx
        public void Property_TransparentColor()
        {
            Console.WriteLine(&quot;Property_TransparentColor()&quot;);
            string infn = path + &quot;Test_PictureTransColor.xlsx&quot;;
            string outfn = Constants.destPath + &quot;Test_PictureTransColorAPI_out.xlsx&quot;;

            Workbook book = new Workbook(infn);
            Worksheet sheet = book.Worksheets[0];
            Picture p = sheet.Pictures[0];
            CellsColor c = p.FormatPicture.TransparentColor;
            Console.WriteLine(c.Color);
            c = book.CreateCellsColor();
            c.Color = Color.Red;
            p.FormatPicture.TransparentColor = c;

            book.Save(outfn);
        }
```

### See Also

* class [CellsColor](../../../aspose.cells/cellscolor/)
* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)



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
// http://www.aspose.com/community/forums/thread/239329.aspx
public void MsoFormatPicture_Property_TransparentColor()
{
    Console.WriteLine("MsoFormatPicture_Property_TransparentColor()");
    string infn = path + "Test_PictureTransColor.xlsx";
    string outfn = Constants.destPath + "Test_PictureTransColorAPI_out.xlsx";

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



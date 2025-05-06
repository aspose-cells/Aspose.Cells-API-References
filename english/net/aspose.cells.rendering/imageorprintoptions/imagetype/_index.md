---
title: ImageOrPrintOptions.ImageType
second_title: Aspose.Cells for .NET API Reference
description: ImageOrPrintOptions property. Gets or sets the format of the generated images. default value PNG
type: docs
url: /net/aspose.cells.rendering/imageorprintoptions/imagetype/
---
## ImageOrPrintOptions.ImageType property

Gets or sets the format of the generated images. default value: PNG.

```csharp
public virtual ImageType ImageType { get; set; }
```

### Examples

```csharp
// Called: new ImageOrPrintOptions() { ImageType = ImageType.Jpeg });
[Test]
        public void Property_ImageType()
        {//content of image should be same with the file name
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;
            cells[0, 1].PutValue(&quot;FirstImage&quot;);
            cells[1, 1].PutValue(&quot;SecondImage&quot;);
            cells[0, 2].PutValue(1);
            wb.Worksheets.Names.Add(&quot;logo&quot;);
            wb.Worksheets.Names[&quot;logo&quot;].RefersTo = &quot;=INDEX(Sheet1!$B$1:$B$4,Sheet1!$C$1)&quot;;
            Picture pic = sheet.Shapes.AddLinkedPicture(0, 0, 40, 200, &quot;&quot;);
            pic.Formula = &quot;logo&quot;;
            sheet.Shapes.UpdateSelectedValue();
            sheet.Shapes[0].ToImage(Constants.destPath + &quot;N55981_First.jpg&quot;,
                new ImageOrPrintOptions() { ImageType = ImageType.Jpeg });

            cells[0, 2].PutValue(2);
            sheet.Shapes.UpdateSelectedValue();
            sheet.Shapes[0].ToImage(Constants.destPath + &quot;N55981_Second.jpg&quot;,
                new ImageOrPrintOptions() { ImageType = ImageType.Jpeg });
        }
```

### See Also

* enum [ImageType](../../../aspose.cells.drawing/imagetype/)
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)



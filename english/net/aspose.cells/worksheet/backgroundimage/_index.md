---
title: Worksheet.BackgroundImage
second_title: Aspose.Cells for .NET API Reference
description: Worksheet property. Gets and sets worksheet background image
type: docs
url: /net/aspose.cells/worksheet/backgroundimage/
---
## Worksheet.BackgroundImage property

Gets and sets worksheet background image.

```csharp
public byte[] BackgroundImage { get; set; }
```

### Examples

```csharp
// Called: workbook.Worksheets[0].BackgroundImage = imgData;
[Test]
        public void Property_BackgroundImage()
        {
            Console.WriteLine("Property_BackgroundImage()");
            string imgfn = path + "TEST_WorksheetBGImage_BMP.bmp";
            string outfn = Constants.destPath + "TEST_WorksheetBGImage_BMP_out.xlsx";

            Workbook workbook = new Workbook();

            FileStream fs = new FileStream(imgfn, FileMode.Open);
            byte[] imgData = new byte[(int)fs.Length];
            fs.Read(imgData, 0, (int)fs.Length);
            workbook.Worksheets[0].BackgroundImage = imgData;
            workbook.Save(outfn);
            fs.Close();
        }
```

### See Also

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



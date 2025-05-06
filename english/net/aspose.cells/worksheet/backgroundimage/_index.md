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
// Called: book.Worksheets[0].BackgroundImage = picData;
[Test]
        public void Property_BackgroundImage()
        {
            Console.WriteLine(&quot;Property_BackgroundImage()&quot;);
            string infn = path + &quot;TEST_SheetBgPicture2.jpg&quot;;
            string outfn = Constants.destPath + &quot;TEST_SheetBgPicture2_out.xlsx&quot;;
            Workbook book = new Workbook();
            FileStream fs = new FileStream(infn, FileMode.Open);
            byte[] picData = new byte[fs.Length];
            fs.Read(picData, 0, (int)fs.Length);
            fs.Close();
            book.Worksheets[0].BackgroundImage = picData;
            book.Save(outfn);
        }
```

### See Also

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



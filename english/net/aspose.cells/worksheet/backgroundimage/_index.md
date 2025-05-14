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
public void Worksheet_Property_BackgroundImage()
{
    Console.WriteLine("Worksheet_Property_BackgroundImage()");
    string infn = path + "TEST_SheetBgPicture2.jpg";
    string outfn = Constants.destPath + "TEST_SheetBgPicture2_out.xlsx";
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



---
title: PageSetup.LeftMargin
second_title: Aspose.Cells for .NET API Reference
description: PageSetup property. Represents the size of the left margin in unit of centimeters
type: docs
url: /net/aspose.cells/pagesetup/leftmargin/
---
## PageSetup.LeftMargin property

Represents the size of the left margin, in unit of centimeters.

```csharp
public double LeftMargin { get; set; }
```

### Examples

```csharp
// Called: sheet.PageSetup.LeftMargin = 0;
public static void PageSetup_Property_LeftMargin()
{
    var book = new Workbook(Constants.TemplatePath + "example.xlsx");

    var sheet = book.Worksheets[0];
    sheet.PageSetup.LeftMargin = 0;
    sheet.PageSetup.RightMargin = 0;
    sheet.PageSetup.TopMargin = 0;
    sheet.PageSetup.BottomMargin = 0;
    var options = new ImageOrPrintOptions
    {
        OnePagePerSheet = true,
        ImageType = ImageType.Emf,
    };

    var sr = new SheetRender(sheet, options);

    using (MemoryStream ms = new MemoryStream())
    {
        sr.ToImage(0, ms);

        ms.Seek(32, SeekOrigin.Begin);
        byte[] buf = new byte[8];
        ms.Read(buf, 0, buf.Length);

        Assert.IsTrue(BitConverter.ToInt32(buf, 0) < (int)(19711 * 1.1));
        Assert.IsTrue(BitConverter.ToInt32(buf, 4) < (int)(13308 * 1.1));
    }
}
```

### See Also

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



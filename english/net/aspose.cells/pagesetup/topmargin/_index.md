---
title: PageSetup.TopMargin
second_title: Aspose.Cells for .NET API Reference
description: PageSetup property. Represents the size of the top margin in unit of centimeters
type: docs
url: /net/aspose.cells/pagesetup/topmargin/
---
## PageSetup.TopMargin property

Represents the size of the top margin, in unit of centimeters.

```csharp
public double TopMargin { get; set; }
```

### Examples

```csharp
// Called: sheet.PageSetup.TopMargin = 0;
[Test]
        public static void Property_TopMargin()
        {
            var book = new Workbook(Constants.TemplatePath + &quot;CELLSNETCORE-226.xlsx&quot;);

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

                Assert.IsTrue(BitConverter.ToInt32(buf, 0) &lt; (int)(19711 * 1.1));
                Assert.IsTrue(BitConverter.ToInt32(buf, 4) &lt; (int)(13308 * 1.1));
            }
        }
```

### See Also

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



---
title: PdfSaveOptions.EmbedStandardWindowsFonts
second_title: Aspose.Cells for .NET API Reference
description: PdfSaveOptions property. True to embed true type fonts. Affects only ASCII characters 32127. Fonts for character codes greater than 127 are always embedded. Fonts are always embedded for PDF/A1a PDF/A1b standard. Default is true
type: docs
url: /net/aspose.cells/pdfsaveoptions/embedstandardwindowsfonts/
---
## PdfSaveOptions.EmbedStandardWindowsFonts property

True to embed true type fonts. Affects only ASCII characters 32-127. Fonts for character codes greater than 127 are always embedded. Fonts are always embedded for PDF/A-1a, PDF/A-1b standard. Default is true.

```csharp
public bool EmbedStandardWindowsFonts { get; set; }
```

### Examples

```csharp
// Called: options.EmbedStandardWindowsFonts = false;
[Test]
        public void Property_EmbedStandardWindowsFonts()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CELLSJAVA-43455.xlsx&quot;);
            PdfSaveOptions options = new PdfSaveOptions();
            options.EmbedStandardWindowsFonts = false;

            using (MemoryStream ms = new MemoryStream())
            {
                workbook.Save(ms, options);

                Assert.IsTrue(ms.Length &gt; 7 * 1024);
            }
        }
```

### See Also

* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



---
title: ImageOrPrintOptions.TextRenderingHint
second_title: Aspose.Cells for .NET API Reference
description: ImageOrPrintOptions property. Specifies the quality of text rendering. The default value is TextRenderingHint.SystemDefault
type: docs
url: /net/aspose.cells.rendering/imageorprintoptions/textrenderinghint/
---
## ImageOrPrintOptions.TextRenderingHint property

Specifies the quality of text rendering. The default value is TextRenderingHint.SystemDefault

```csharp
public TextRenderingHint TextRenderingHint { get; set; }
```

### Examples

```csharp
// Called: TextRenderingHint = TextRenderingHint.AntiAlias,
[Test]
        public void Property_TextRenderingHint()
        {
            var options = new ImageOrPrintOptions
            {
                ImageType = ImageType.OfficeCompatibleEmf,
                OnlyArea = false,   // copy as picture - as shown when printed
                TextRenderingHint = TextRenderingHint.AntiAlias,
                OnePagePerSheet = true,
                Transparent = true,
            };

            Workbook wb = new Workbook();
            wb.Worksheets[0].Cells["A1"].PutValue("test");
            wb.Worksheets[0].PageSetup.PrintArea = "A1:A1";
            Worksheet ws = wb.Worksheets[0];
            ws.PageSetup.LeftMargin = ws.PageSetup.RightMargin
                = ws.PageSetup.TopMargin = ws.PageSetup.BottomMargin
                = ws.PageSetup.HeaderMargin = ws.PageSetup.FooterMargin = 0;

            MemoryStream ms = new MemoryStream();
            new SheetRender(ws, options).ToImage(0, ms);

            //GdiPlusGetDC record byte
            byte[] getDCData = new byte[] { 0x04, 0x40, 0x00, 0x00, 0x0C, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00 };

            Assert.IsTrue(FindPosition(ms, getDCData) > -1);
        }
```

### See Also

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)



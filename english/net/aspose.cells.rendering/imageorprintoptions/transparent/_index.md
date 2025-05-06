---
title: ImageOrPrintOptions.Transparent
second_title: Aspose.Cells for .NET API Reference
description: ImageOrPrintOptions property. Indicates if the background of generated image should be transparent
type: docs
url: /net/aspose.cells.rendering/imageorprintoptions/transparent/
---
## ImageOrPrintOptions.Transparent property

Indicates if the background of generated image should be transparent.

```csharp
public bool Transparent { get; set; }
```

### Remarks

The default value is false. That means the background of the generated images is white.

### Examples

```csharp
// Called: Transparent = true,
[Test]
        public void Property_Transparent()
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
            wb.Worksheets[0].Cells[&quot;A1&quot;].PutValue(&quot;test&quot;);
            wb.Worksheets[0].PageSetup.PrintArea = &quot;A1:A1&quot;;
            Worksheet ws = wb.Worksheets[0];
            ws.PageSetup.LeftMargin = ws.PageSetup.RightMargin
                = ws.PageSetup.TopMargin = ws.PageSetup.BottomMargin
                = ws.PageSetup.HeaderMargin = ws.PageSetup.FooterMargin = 0;

            MemoryStream ms = new MemoryStream();
            new SheetRender(ws, options).ToImage(0, ms);

            //GdiPlusGetDC record byte
            byte[] getDCData = new byte[] { 0x04, 0x40, 0x00, 0x00, 0x0C, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00 };

            Assert.IsTrue(FindPosition(ms, getDCData) &gt; -1);
        }
```

### See Also

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)



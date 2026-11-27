---
title: "ImageOrPrintOptions.SvgCssPrefix"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ImageOrPrintOptions-egenskap. Hämtar och anger prefixet för css-namnet i svg, standardvärdet är en tom sträng"
type: docs
url: /sv/net/aspose.cells.rendering/imageorprintoptions/svgcssprefix/
---
## ImageOrPrintOptions.SvgCssPrefix property

Hämtar och anger prefixet för css-namnet i svg, standardvärdet är en tom sträng.

```csharp
[Obsolete("Use SvgImageOptions.CssPrefix property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public string SvgCssPrefix { get; set; }
```

### Anmärkningar

OBS: Denna medlem är nu föråldrad. Använd i stället [`CssPrefix`](../../svgimageoptions/cssprefix/). Denna egenskap kommer att tas bort 12 månader senare från och med april 2025. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsPropertySvgCssPrefixDemo
    {
        public static void Run()
        {
            string prefix = "custom_prefix_";

            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Cells["A1"].PutValue("SVG CSS Prefix Test");

            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = Aspose.Cells.Drawing.ImageType.Svg;
            options.OnePagePerSheet = true;
            options.SvgCssPrefix = prefix;

            SheetRender renderer = new SheetRender(workbook.Worksheets[0], options);
            using (MemoryStream stream = new MemoryStream())
            {
                renderer.ToImage(0, stream);
                stream.Position = 0;
                using (StreamReader reader = new StreamReader(stream))
                {
                    string svgContent = reader.ReadToEnd();
                    Console.WriteLine("SVG contains CSS prefix: " + svgContent.Contains(prefix + "f"));
                }
            }
        }
    }
}
```

### Se även

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)



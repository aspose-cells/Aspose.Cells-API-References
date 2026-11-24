---
title: "ImageOrPrintOptions.SvgCssPrefix"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ImageOrPrintOptions-Eigenschaft. Ruft das Präfix des CSS-Namens in SVG ab und legt es fest, der Standardwert ist eine leere Zeichenkette"
type: docs
url: /de/net/aspose.cells.rendering/imageorprintoptions/svgcssprefix/
---
## ImageOrPrintOptions.SvgCssPrefix property

Ermittelt und legt das Präfix des CSS-Namens in SVG fest, der Standardwert ist eine leere Zeichenkette.

```csharp
[Obsolete("Use SvgImageOptions.CssPrefix property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public string SvgCssPrefix { get; set; }
```

### Hinweise

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen [`CssPrefix`](../../svgimageoptions/cssprefix/). Diese Eigenschaft wird 12 Monate später, seit April 2025, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erlebt haben.

### Beispiele

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

### Siehe auch

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)



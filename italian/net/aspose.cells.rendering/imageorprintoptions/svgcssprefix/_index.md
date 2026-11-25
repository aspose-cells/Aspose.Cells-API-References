---
title: "ImageOrPrintOptions.SvgCssPrefix"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ImageOrPrintOptions. Ottiene e imposta il prefisso del nome css in svg. Il valore predefinito è una stringa vuota"
type: docs
url: /it/net/aspose.cells.rendering/imageorprintoptions/svgcssprefix/
---
## ImageOrPrintOptions.SvgCssPrefix property

Ottiene e imposta il prefisso del nome CSS in SVG, il valore predefinito è una stringa vuota.

```csharp
[Obsolete("Use SvgImageOptions.CssPrefix property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public string SvgCssPrefix { get; set; }
```

### Osservazioni

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare [`CssPrefix`](../../svgimageoptions/cssprefix/). Questa proprietà sarà rimossa tra 12 mesi a partire da aprile 2025. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

### Esempi

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

### Vedi anche

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)



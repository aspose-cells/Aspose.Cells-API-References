---
title: "ImageOrPrintOptions.SvgCssPrefix"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ImageOrPrintOptions. Obtiene y establece el prefijo del nombre css en svg. El valor predeterminado es una cadena vacía"
type: docs
url: /es/net/aspose.cells.rendering/imageorprintoptions/svgcssprefix/
---
## ImageOrPrintOptions.SvgCssPrefix property

Obtiene y establece el prefijo del nombre CSS en SVG, el valor predeterminado es una cadena vacía.

```csharp
[Obsolete("Use SvgImageOptions.CssPrefix property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public string SvgCssPrefix { get; set; }
```

### Observaciones

NOTA: Este miembro está ahora obsoleto. En su lugar, utilice [`CssPrefix`](../../svgimageoptions/cssprefix/). Esta propiedad será eliminada 12 meses después desde abril de 2025. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

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

### Ver también

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)



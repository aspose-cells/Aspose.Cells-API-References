---
title: "ImageOrPrintOptions.SVGFitToViewPort"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ImageOrPrintOptions. si esta propiedad es verdadera, el svg generado se ajustará al viewport"
type: docs
url: /es/net/aspose.cells.rendering/imageorprintoptions/svgfittoviewport/
---
## ImageOrPrintOptions.SVGFitToViewPort property

Si esta propiedad es verdadera, el SVG generado se ajustará al viewport.

```csharp
[Obsolete("Use SvgImageOptions.FitToViewPort property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool SVGFitToViewPort { get; set; }
```

### Observaciones

NOTA: Este miembro está ahora obsoleto. En su lugar, utilice [`FitToViewPort`](../../svgimageoptions/fittoviewport/). Esta propiedad será eliminada 12 meses después a partir de abril de 2025. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsPropertySVGFitToViewPortDemo
    {
        public static void Run()
        {
            // Crea un nuevo libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de muestra a las celdas
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["B1"].PutValue("Quantity");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B3"].PutValue(15);
            
            // Crear opciones de imagen para la salida SVG
            ImageOrPrintOptions opts = new ImageOrPrintOptions();
            opts.ImageType = Aspose.Cells.Drawing.ImageType.Svg;
            opts.OnePagePerSheet = true;
            opts.SVGFitToViewPort = true; // This is the key property being demonstrated
            
            // Renderizar la hoja de cálculo a una imagen SVG
            SheetRender sr = new SheetRender(worksheet, opts);
            sr.ToImage(0, "output.svg");
            
            Console.WriteLine("SVG file with SVGFitToViewPort=true created successfully.");
        }
    }
}
```

### Ver también

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)



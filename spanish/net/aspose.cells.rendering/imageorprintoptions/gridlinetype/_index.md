---
title: "ImageOrPrintOptions.GridlineType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ImageOrPrintOptions. Obtiene o establece el tipo de línea de cuadrícula"
type: docs
url: /es/net/aspose.cells.rendering/imageorprintoptions/gridlinetype/
---
## ImageOrPrintOptions.GridlineType property

Obtiene o establece el tipo de línea de cuadrícula.

```csharp
public GridlineType GridlineType { get; set; }
```

### Observaciones

El valor predeterminado es tipo Dotted.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Rendering;
    using System;

    public class ImageOrPrintOptionsPropertyGridlineTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo y rellenar con datos de muestra
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Book");
            worksheet.Cells["B2"].PutValue("$19.99");
            worksheet.Cells["A3"].PutValue("Pen");
            worksheet.Cells["B3"].PutValue("$2.99");

            // Crear una instancia de ImageOrPrintOptions
            ImageOrPrintOptions imageOptions = new ImageOrPrintOptions
            {
                ImageType = ImageType.Png,
                GridlineType = GridlineType.Dotted // Use valid enum value
            };

            // Mostrar el tipo de línea de cuadrícula actual
            Console.WriteLine("Initial GridlineType: " + imageOptions.GridlineType);

            // Renderizar la hoja de cálculo con el tipo de línea de cuadrícula inicial
            SheetRender solidLineRenderer = new SheetRender(worksheet, imageOptions);
            solidLineRenderer.ToImage(0, "SolidGridlines.png");

            // Cambiar el tipo de línea de cuadrícula y volver a renderizar
            imageOptions.GridlineType = GridlineType.Hair; // Use valid enum value
            Console.WriteLine("\nModified GridlineType: " + imageOptions.GridlineType);

            SheetRender dashedLineRenderer = new SheetRender(worksheet, imageOptions);
            dashedLineRenderer.ToImage(0, "DashedGridlines.png");

            Console.WriteLine("Generated images demonstrate different gridline styles.");
        }
    }
}
```

### Ver también

* enum [GridlineType](../../../aspose.cells/gridlinetype/)
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)



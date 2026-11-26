---
title: "ImageOrPrintOptions.VerticalResolution"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ImageOrPrintOptions. Obtiene o establece la resolución vertical para las imágenes generadas en puntos por pulgada"
type: docs
url: /es/net/aspose.cells.rendering/imageorprintoptions/verticalresolution/
---
## ImageOrPrintOptions.VerticalResolution property

Obtiene o establece la resolución vertical para las imágenes generadas, en puntos por pulgada.

```csharp
public int VerticalResolution { get; set; }
```

### Observaciones

El valor predeterminado es 96.

Configurar [`HorizontalResolution`](../horizontalresolution/) y `VerticalResolution` afecta el ancho y la altura de la imagen de salida en píxeles.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
using Aspose.Cells.Drawing;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsPropertyVerticalResolutionDemo
    {
        public static void Run()
        {
            // Crea un nuevo libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de muestra y crear un gráfico
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("Product A");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("Product B");
            worksheet.Cells["B3"].PutValue(200);
            
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            // Crear opciones de imagen con una resolución vertical específica
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = ImageType.Png;
            options.VerticalResolution = 300; // Setting vertical resolution to 300 DPI
            options.HorizontalResolution = 300; // For consistency, setting horizontal resolution too

            // Guardar el gráfico como imagen con la resolución especificada
            chart.ToImage("output_chart.png", options);
            
            Console.WriteLine("Chart saved as image with vertical resolution of 300 DPI.");
        }
    }
}
```

### Ver también

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)



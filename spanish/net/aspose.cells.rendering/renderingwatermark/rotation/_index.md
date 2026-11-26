---
title: "RenderingWatermark.Rotation"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad RenderingWatermark. Obtiene o establece la rotación de la marca de agua en grados"
type: docs
url: /es/net/aspose.cells.rendering/renderingwatermark/rotation/
---
## RenderingWatermark.Rotation property

Obtiene o establece la rotación de la marca de agua en grados.

```csharp
public float Rotation { get; set; }
```

### Ejemplos

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class RenderingWatermarkPropertyRotationDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample data for watermark demo");

            // Crear fuente para la marca de agua
            RenderingFont font = new RenderingFont("Arial", 72);
            font.Color = Color.FromArgb(128, 0, 0, 255);
            font.Bold = true;

            // Crear marca de agua con rotación
            RenderingWatermark watermark = new RenderingWatermark("ROTATED WATERMARK", font);
            watermark.Rotation = 45; // 45 degree rotation
            watermark.Opacity = 0.5f;
            watermark.IsBackground = true;

            // Establecer opciones de guardado PDF con marca de agua
            PdfSaveOptions options = new PdfSaveOptions();
            options.Watermark = watermark;

            // Guardar con marca de agua
            workbook.Save("WatermarkRotationDemo.pdf", options);
        }
    }
}
```

### Ver también

* class [RenderingWatermark](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)



---
title: "TextureFill.ImageData"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad TextureFill. Obtiene y establece los datos de imagen del relleno"
type: docs
url: /es/net/aspose.cells.drawing/texturefill/imagedata/
---
## TextureFill.ImageData property

Obtiene y establece los datos de imagen del relleno.

```csharp
public byte[] ImageData { get; set; }
```

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class TextureFillPropertyImageDataDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Añade un gráfico
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 5, 15, 15);
            Chart chart = worksheet.Charts[chartIndex];

            // Establecer tipo de relleno de textura
            chart.ChartArea.Area.FillFormat.FillType = FillType.Texture;

            // Cargar datos de la imagen
            byte[] imageData = File.ReadAllBytes("texture.png");

            // Establecer datos de imagen para el relleno de textura
            chart.ChartArea.Area.FillFormat.TextureFill.ImageData = imageData;

            // Guarda el libro de trabajo
            workbook.Save("TextureFillDemo.xlsx");
        }
    }
}
```

### Ver también

* class [TextureFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)



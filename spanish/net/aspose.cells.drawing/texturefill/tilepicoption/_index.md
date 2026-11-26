---
title: "TextureFill.TilePicOption"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad TextureFill. Obtiene o establece la opción de imagen de mosaico"
type: docs
url: /es/net/aspose.cells.drawing/texturefill/tilepicoption/
---
## TextureFill.TilePicOption property

Obtiene o establece la opción de mosaico de imagen.

```csharp
public TilePicOption TilePicOption { get; set; }
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
    public class TextureFillPropertyTilePicOptionDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Añade un gráfico
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 5, 15, 15);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];

            // Establecer relleno de textura con imagen
            chart.ChartArea.Area.FillFormat.FillType = FillType.Texture;
            byte[] imageData = File.ReadAllBytes("texture.png");
            chart.ChartArea.Area.FillFormat.TextureFill.ImageData = imageData;

            // Configurar opciones de mosaico
            chart.ChartArea.Area.FillFormat.TextureFill.TilePicOption = new TilePicOption();
            chart.ChartArea.Area.FillFormat.TextureFill.TilePicOption.ScaleX = 50;
            chart.ChartArea.Area.FillFormat.TextureFill.TilePicOption.ScaleY = 50;
            chart.ChartArea.Area.FillFormat.TextureFill.TilePicOption.OffsetX = 10;
            chart.ChartArea.Area.FillFormat.TextureFill.TilePicOption.OffsetY = 10;

            // Guarda el libro de trabajo
            workbook.Save("TextureFillDemo.xlsx");
        }
    }
}
```

### Ver también

* class [TilePicOption](../../tilepicoption/)
* class [TextureFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)



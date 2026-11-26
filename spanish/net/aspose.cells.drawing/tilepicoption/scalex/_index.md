---
title: "TilePicOption.ScaleX"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad TilePicOption. Obtiene o establece la escala X para la imagen de mosaico"
type: docs
url: /es/net/aspose.cells.drawing/tilepicoption/scalex/
---
## TilePicOption.ScaleX property

Obtiene o establece la escala X para la imagen de mosaico.

```csharp
public double ScaleX { get; set; }
```

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TilePicOptionPropertyScaleXDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de muestra y crear un gráfico
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:A3", true);

            // Establecer relleno de textura con imagen
            string imagePath = Path.Combine(Environment.GetFolderPath(Environment.SpecialFolder.Desktop), "texture.png");
            byte[] imageData = File.ReadAllBytes(imagePath);
            
            chart.ChartArea.Area.FillFormat.FillType = FillType.Texture;
            chart.ChartArea.Area.FillFormat.TextureFill.ImageData = imageData;
            chart.ChartArea.Area.FillFormat.TextureFill.TilePicOption = new TilePicOption();
            
            // Demostrar la propiedad ScaleX
            chart.ChartArea.Area.FillFormat.TextureFill.TilePicOption.ScaleX = 50; // 50% horizontal scaling
            chart.ChartArea.Area.FillFormat.TextureFill.TilePicOption.ScaleY = 75; // 75% vertical scaling

            // Guarda el libro de trabajo
            workbook.Save(Path.Combine(Environment.GetFolderPath(Environment.SpecialFolder.Desktop), "ScaleXDemo.xlsx"));
        }
    }
}
```

### Ver también

* class [TilePicOption](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)



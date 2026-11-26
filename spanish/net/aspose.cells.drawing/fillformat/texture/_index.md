---
title: "FillFormat.Texture"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad FillFormat. Representa el tipo de textura para el relleno especificado"
type: docs
url: /es/net/aspose.cells.drawing/fillformat/texture/
---
## FillFormat.Texture property

Representa el tipo de textura para el relleno especificado.

```csharp
public TextureType Texture { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class FillFormatPropertyTextureDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo para el gráfico
            sheet.Cells["A1"].PutValue("Item");
            sheet.Cells["A2"].PutValue("Product A");
            sheet.Cells["A3"].PutValue("Product B");
            sheet.Cells["A4"].PutValue("Product C");
            sheet.Cells["B1"].PutValue("Sales");
            sheet.Cells["B2"].PutValue(1000);
            sheet.Cells["B3"].PutValue(2000);
            sheet.Cells["B4"].PutValue(3000);

            // Añade un gráfico
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = sheet.Charts[chartIndex];
            
            // Establecer rango de datos del gráfico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Establece la textura para el tercer punto de la primera serie
            ChartPoint point = chart.NSeries[0].Points[2];
            point.Area.FillFormat.Texture = TextureType.Oak;

            // Guarda el libro de trabajo
            workbook.Save("FillFormatTextureDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [TextureType](../../texturetype/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)



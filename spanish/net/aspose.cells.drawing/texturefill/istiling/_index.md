---
title: "TextureFill.IsTiling"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad TextureFill. Indica si la imagen se repite como textura"
type: docs
url: /es/net/aspose.cells.drawing/texturefill/istiling/
---
## TextureFill.IsTiling property

Indica si la imagen se repite como textura.

```csharp
public bool IsTiling { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TextureFillPropertyIsTilingDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Añade un gráfico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Establecer datos del gráfico
            chart.NSeries.Add("A1:B3", true);
            
            // Establecer relleno de textura para el área del gráfico
            chart.PlotArea.Area.FillFormat.Texture = TextureType.BlueTissuePaper;
            
            // Establecer la propiedad IsTiling
            chart.PlotArea.Area.FillFormat.TextureFill.IsTiling = true;
            
            // Verificar y mostrar el valor de IsTiling
            Console.WriteLine("IsTiling: " + chart.PlotArea.Area.FillFormat.TextureFill.IsTiling);
            
            // Guarda el libro de trabajo
            workbook.Save("TextureFillIsTilingDemo.xlsx");
        }
    }
}
```

### Ver también

* class [TextureFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)



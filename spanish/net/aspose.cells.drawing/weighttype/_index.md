---
title: "Enumeración WeightType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enumeración Aspose.Cells.Drawing.WeightType. Enumera los tipos de grosor para el borde de una imagen o una línea de gráfico"
type: docs
url: /es/net/aspose.cells.drawing/weighttype/
---
## WeightType enumeration

Enumera los tipos de peso para el borde de una imagen o una línea de gráfico.

```csharp
public enum WeightType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| HairLine | `-1` | Representa el grosor de una línea muy fina. |
| MediumLine | `1` | Representa el grosor de una línea media. |
| SingleLine | `0` | Representa el grosor de una línea simple. |
| WideLine | `2` | Representa el grosor de una línea ancha. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassWeightTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agrega un gráfico y obtén su área de gráfico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 5, 15, 15);
            Chart chart = worksheet.Charts[chartIndex];
            ChartArea chartArea = chart.ChartArea;
            
            // Establece el tipo de grosor del borde
            chartArea.Border.Weight = WeightType.WideLine;
            
            // Verifica el tipo de grosor
            Console.WriteLine("Chart Area Border Weight: " + chartArea.Border.Weight);
            
            // Guarda el libro de trabajo
            workbook.Save("WeightTypeDemo.xlsx");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)



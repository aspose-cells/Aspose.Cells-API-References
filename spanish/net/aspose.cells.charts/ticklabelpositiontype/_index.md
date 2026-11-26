---
title: "Enumeración TickLabelPositionType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.Charts.TickLabelPositionType enum. Representa el tipo de posición de las etiquetas de marcas de graduación en el eje especificado"
type: docs
url: /es/net/aspose.cells.charts/ticklabelpositiontype/
---
## TickLabelPositionType enumeration

Representa el tipo de posición de las etiquetas de marcas de graduación en el eje especificado.

```csharp
public enum TickLabelPositionType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| High | `0` | El tipo de posición es alto. |
| Low | `1` | El tipo de posición es bajo. |
| NextToAxis | `2` | El tipo de posición es al lado del eje. |
| None | `3` | El tipo de posición es ninguno. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class TickLabelPositionTypeDemo
    {
        public static void TickLabelPositionTypeExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Agregar una nueva hoja de cálculo al libro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar algunos datos de ejemplo a la hoja de cálculo
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(4);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(50);
            
            // Agregar un gráfico a la hoja de cálculo
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 25, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Agrega NSeries (fuente de datos del gráfico) al gráfico que abarca desde la celda "A1" hasta "B3"
            chart.NSeries.Add("A1:B3", true);
            
            // Accede al eje de categorías
            Axis categoryAxis = chart.CategoryAxis;
            
            // Establece la posición de la etiqueta de graduación a Alto
            categoryAxis.TickLabelPosition = TickLabelPositionType.High;
            
            // Guarda el libro de trabajo
            workbook.Save("TickLabelPositionTypeExample.xlsx");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)



---
title: "Axis.TickLabels"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Axis. Devuelve un objeto TickLabels que representa las etiquetas de marcas de graduación para el eje especificado"
type: docs
url: /es/net/aspose.cells.charts/axis/ticklabels/
---
## Axis.TickLabels property

Devuelve un objeto `TickLabels` que representa las etiquetas de marcas de graduación para el eje especificado.

```csharp
public TickLabels TickLabels { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyTickLabelsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            
            // Agregar gráfico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Establecer origen de datos del Chart
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // Acceder a las etiquetas de marca del eje de categorías
            Aspose.Cells.Charts.Axis axis = chart.CategoryAxis;
            axis.TickLabels.Font.IsBold = true;
            axis.TickLabels.Font.Color = System.Drawing.Color.Red;
            axis.TickLabels.RotationAngle = 45;
            
            // Guarda el libro de trabajo
            workbook.Save("AxisPropertyTickLabelsDemo_out.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ver también

* class [TickLabels](../../ticklabels/)
* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)



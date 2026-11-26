---
title: "ChartFrame.IsAutomaticSize"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ChartFrame. Indica si el marco del gráfico tiene tamaño automático"
type: docs
url: /es/net/aspose.cells.charts/chartframe/isautomaticsize/
---
## ChartFrame.IsAutomaticSize property

Indica si el marco del gráfico tiene tamaño automático.

```csharp
public virtual bool IsAutomaticSize { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartFramePropertyIsAutomaticSizeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo para el gráfico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B4"].PutValue(30);

            // Añade un gráfico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Establecer origen de datos del Chart
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Acceder a la leyenda y demostrar la propiedad IsAutomaticSize
            Aspose.Cells.Charts.Legend legend = chart.Legend;
            
            // Establecer el tamaño automático a false y mostrar el valor
            legend.IsAutomaticSize = false;
            Console.WriteLine("Legend Automatic Size: " + legend.IsAutomaticSize);
            
            // Establecer el tamaño automático a true y mostrar el valor
            legend.IsAutomaticSize = true;
            Console.WriteLine("Legend Automatic Size: " + legend.IsAutomaticSize);
        }
    }
}
```

### Ver también

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)



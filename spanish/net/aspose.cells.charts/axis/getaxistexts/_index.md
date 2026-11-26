---
title: "Axis.GetAxisTexts"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Axis. Obtiene las etiquetas del eje después de llamar al método Chart.Calculate"
type: docs
url: /es/net/aspose.cells.charts/axis/getaxistexts/
---
## Axis.GetAxisTexts method

Obtiene las etiquetas del eje después de llamar al método Chart.Calculate().

```csharp
public string[] GetAxisTexts()
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisMethodGetAxisTextsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo para el gráfico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(8000);
            worksheet.Cells["B3"].PutValue(4000);
            worksheet.Cells["B4"].PutValue(-8000);

            // Añade un gráfico
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Establecer rango de datos del gráfico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // Calcular gráfico
            chart.Calculate();
            
            // Obtener etiquetas del eje
            string[] labels = chart.ValueAxis.GetAxisTexts();
            
            // Mostrar las etiquetas
            Console.WriteLine("Value Axis Labels:");
            foreach (string label in labels)
            {
                Console.WriteLine(label);
            }
        }
    }
}
```

### Ver también

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)



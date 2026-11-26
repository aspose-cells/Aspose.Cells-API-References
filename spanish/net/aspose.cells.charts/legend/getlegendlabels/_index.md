---
title: "Legend.GetLegendLabels"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Legend. Obtiene las etiquetas de las entradas de la leyenda después de llamar al método Chart.Calculate"
type: docs
url: /es/net/aspose.cells.charts/legend/getlegendlabels/
---
## Legend.GetLegendLabels method

Obtiene las etiquetas de las entradas de la leyenda después de llamar al método Chart.Calculate().

```csharp
public string[] GetLegendLabels()
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class LegendMethodGetLegendLabelsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo para el gráfico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            
            // Añade un gráfico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Establecer rango de datos del gráfico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // Calcular gráfico
            chart.Calculate();
            
            // Obtener etiquetas de la leyenda
            string[] legendLabels = chart.Legend.GetLegendLabels();
            
            // Mostrar etiquetas de la leyenda
            Console.WriteLine("Legend Labels:");
            foreach (string label in legendLabels)
            {
                Console.WriteLine(label);
            }
        }
    }
}
```

### Ver también

* class [Legend](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)



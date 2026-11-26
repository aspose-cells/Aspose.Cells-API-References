---
title: "Chart.Name"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad del gráfico. Obtiene y establece el nombre del gráfico"
type: docs
url: /es/net/aspose.cells.charts/chart/name/
---
## Chart.Name property

Obtiene y establece el nombre del gráfico.

```csharp
public string Name { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyNameDemo
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
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Establecer rango de datos del gráfico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Mostrar el nombre del gráfico
            Console.WriteLine("Chart Name: " + chart.Name);

            // Agregar otro gráfico y mostrar su nombre
            int chartIndex2 = worksheet.Charts.Add(ChartType.Pie, 20, 0, 30, 5);
            Aspose.Cells.Charts.Chart chart2 = worksheet.Charts[chartIndex2];
            chart2.NSeries.Add("B2:B4", true);
            chart2.NSeries.CategoryData = "A2:A4";
            Console.WriteLine("Second Chart Name: " + chart2.Name);
        }
    }
}
```

### Ver también

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)



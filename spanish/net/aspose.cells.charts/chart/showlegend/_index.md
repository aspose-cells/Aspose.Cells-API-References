---
title: "Chart.ShowLegend"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Chart. Obtiene o establece un valor que indica si la leyenda del gráfico se mostrará. El valor predeterminado es true"
type: docs
url: /es/net/aspose.cells.charts/chart/showlegend/
---
## Chart.ShowLegend property

Obtiene o establece un valor que indica si se mostrará la leyenda del gráfico. El valor predeterminado es true.

```csharp
public bool ShowLegend { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyShowLegendDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            sheet.Cells["A1"].PutValue("Item");
            sheet.Cells["A2"].PutValue("Apple");
            sheet.Cells["A3"].PutValue("Orange");
            sheet.Cells["A4"].PutValue("Banana");
            sheet.Cells["B1"].PutValue("Quantity");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["B3"].PutValue(20);
            sheet.Cells["B4"].PutValue(30);

            // Añade un gráfico
            int chartIndex = sheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = sheet.Charts[chartIndex];
            
            // Establecer rango de datos del gráfico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Mostrar leyenda por defecto (true)
            Console.WriteLine("Legend initially visible: " + chart.ShowLegend);
            
            // Ocultar la leyenda
            chart.ShowLegend = false;
            Console.WriteLine("Legend after setting to false: " + chart.ShowLegend);
            
            // Guarda el libro de trabajo
            workbook.Save("ChartLegendExample.xlsx");
        }
    }
}
```

### Ver también

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)



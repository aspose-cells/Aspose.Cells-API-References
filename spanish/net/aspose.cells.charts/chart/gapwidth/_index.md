---
title: "Chart.GapWidth"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad del gráfico. Devuelve o establece el espacio entre grupos de barras o columnas como un porcentaje del ancho de la barra o columna. El valor de esta propiedad debe estar entre 0 y 500"
type: docs
url: /es/net/aspose.cells.charts/chart/gapwidth/
---
## Chart.GapWidth property

Devuelve o establece el espacio entre grupos de barras o columnas, como un porcentaje del ancho de la barra o columna. El valor de esta propiedad debe estar entre 0 y 500.

```csharp
public int GapWidth { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyGapWidthDemo
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
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Agregar un gráfico de columnas
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Establecer rango de datos del gráfico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Demostrar la propiedad GapWidth
            Console.WriteLine("Original GapWidth: " + chart.GapWidth);
            chart.GapWidth = 150; // Set gap width to 150% of default
            Console.WriteLine("Modified GapWidth: " + chart.GapWidth);

            // Guarda el libro de trabajo
            workbook.Save("ChartGapWidthDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ver también

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)



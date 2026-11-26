---
title: "SeriesLayoutProperties.Subtotals"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad SeriesLayoutProperties. Representa el índice de un punto de datos subtotal"
type: docs
url: /es/net/aspose.cells.charts/serieslayoutproperties/subtotals/
---
## SeriesLayoutProperties.Subtotals property

Representa el índice de un punto de datos subtotal.

```csharp
public int[] Subtotals { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesLayoutPropertiesPropertySubtotalsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo para el gráfico
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["A4"].PutValue("C");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["B3"].PutValue(20);
            sheet.Cells["B4"].PutValue(30);

            // Añade un gráfico
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = sheet.Charts[chartIndex];

            // Establecer rango de datos del gráfico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Establezca subtotales para la primera serie
            chart.NSeries[0].LayoutProperties.Subtotals = new int[] { 0, 3 };

            // Verifique que los subtotales se hayan configurado correctamente
            Console.WriteLine("Subtotal at index 0: " + chart.NSeries[0].LayoutProperties.Subtotals[0]);
            Console.WriteLine("Subtotal at index 1: " + chart.NSeries[0].LayoutProperties.Subtotals[1]);

            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [SeriesLayoutProperties](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)



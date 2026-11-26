---
title: "Series.Values"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Series. Representa los valores Y de esta serie de gráfico"
type: docs
url: /es/net/aspose.cells.charts/series/values/
---
## Series.Values property

Representa los valores Y de esta serie de gráfico.

```csharp
public string Values { get; set; }
```

### Observaciones

Para obtener los valores reales (correspondientes a cada punto de esta serie) definidos por esta propiedad, por favor use [`PointValues`](../pointvalues/).

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyValuesDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de muestra a las celdas
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Series1");
            worksheet.Cells["C1"].PutValue("Series2");
            
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            
            worksheet.Cells["C2"].PutValue(15);
            worksheet.Cells["C3"].PutValue(25);
            worksheet.Cells["C4"].PutValue(35);

            // Añade un gráfico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Agregar serie usando la propiedad Values
            chart.NSeries.Add("=Sheet1!$B$2:$B$4", true);
            chart.NSeries.Add("=Sheet1!$C$2:$C$4", true);

            // Establecer datos de categoría
            chart.NSeries.CategoryData = "=Sheet1!$A$2:$A$4";

            // Mostrar la propiedad Values para cada serie
            Console.WriteLine("Series 1 Values: " + chart.NSeries[0].Values);
            Console.WriteLine("Series 2 Values: " + chart.NSeries[1].Values);

            // Guarda el libro de trabajo
            workbook.Save("SeriesPropertyValuesDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)



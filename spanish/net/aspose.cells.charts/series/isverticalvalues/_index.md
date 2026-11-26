---
title: "Series.IsVerticalValues"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Series. Indica si la fuente de datos es vertical"
type: docs
url: /es/net/aspose.cells.charts/series/isverticalvalues/
---
## Series.IsVerticalValues property

Indica si la fuente de datos es vertical.

```csharp
public bool IsVerticalValues { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyIsVerticalValuesDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            for (int i = 2; i <= 10; i++)
            {
                worksheet.Cells["A" + i].PutValue("Cat " + (i-1));
                worksheet.Cells["B" + i].PutValue(i * 10);
            }

            // Agregar gráfico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Agregar serie con valores verticales
            chart.NSeries.Add("A1:B10", true);
            
            // Demostrar la propiedad IsVerticalValues (solo lectura)
            Console.WriteLine("IsVerticalValues for first series: " + chart.NSeries[0].IsVerticalValues);
            
            // Para cambiar la orientación, necesitamos recrear la serie con parámetros diferentes
            chart.NSeries.Clear();
            chart.NSeries.Add("A1:B10", false);
            Console.WriteLine("IsVerticalValues after recreation: " + chart.NSeries[0].IsVerticalValues);
        }
    }
}
```

### Ver también

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)



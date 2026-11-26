---
title: "Series.CountOfDataValues"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Series. Obtiene el número de valores de datos"
type: docs
url: /es/net/aspose.cells.charts/series/countofdatavalues/
---
## Series.CountOfDataValues property

Obtiene el número de los valores de datos.

```csharp
public int CountOfDataValues { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyCountOfDataValuesDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de muestra a las celdas
            for (int i = 0; i < 4; i++)
            {
                worksheet.Cells[i, 0].PutValue(i + 1); // A1:A4 with values 1-4
            }

            // Crear un gráfico
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Agregar series usando el rango de datos
            chart.NSeries.Add("A1:A4", true);
            
            // Mostrar el recuento de valores de datos en la primera serie
            Console.WriteLine("Count of data values in series: " + chart.NSeries[0].CountOfDataValues);
            
            // Guarda el libro de trabajo
            workbook.Save("SeriesPropertyCountOfDataValuesDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)



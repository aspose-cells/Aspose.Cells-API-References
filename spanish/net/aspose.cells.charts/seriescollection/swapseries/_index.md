---
title: "SeriesCollection.SwapSeries"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método SeriesCollection. Cambia directamente el orden de las dos series"
type: docs
url: /es/net/aspose.cells.charts/seriescollection/swapseries/
---
## SeriesCollection.SwapSeries method

Cambia directamente el orden de las dos series.

```csharp
public void SwapSeries(int sourceIndex, int destIndex)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sourceIndex | Int32 | El índice actual |
| destIndex | Int32 | El índice de destino |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesCollectionMethodSwapSeriesWithInt32Int32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo para el gráfico
            worksheet.Cells["A1"].PutValue("Series 1");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(20);
            worksheet.Cells["A4"].PutValue(30);
            
            worksheet.Cells["B1"].PutValue("Series 2");
            worksheet.Cells["B2"].PutValue(5);
            worksheet.Cells["B3"].PutValue(10);
            worksheet.Cells["B4"].PutValue(15);
            
            worksheet.Cells["C1"].PutValue("Series 3");
            worksheet.Cells["C2"].PutValue(8);
            worksheet.Cells["C3"].PutValue(16);
            worksheet.Cells["C4"].PutValue(24);

            // Añade un gráfico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Establecer rango de datos del gráfico
            chart.NSeries.Add("A1:C4", true);
            
            // Obtener la colección de series
            Aspose.Cells.Charts.SeriesCollection sc = chart.NSeries;
            
            // Imprimir los nombres originales de las series
            Console.WriteLine("Original Series Order:");
            for (int i = 0; i < sc.Count; i++)
            {
                Console.WriteLine($"Series {i}: {sc[i].Name}");
            }
            
            // Intercambiar series 0 y 1
            sc.SwapSeries(0, 1);
            Console.WriteLine("\nAfter swapping series 0 and 1:");
            for (int i = 0; i < sc.Count; i++)
            {
                Console.WriteLine($"Series {i}: {sc[i].Name}");
            }
            
            // Intercambiar series 2 y 0
            sc.SwapSeries(2, 0);
            Console.WriteLine("\nAfter swapping series 2 and 0:");
            for (int i = 0; i < sc.Count; i++)
            {
                Console.WriteLine($"Series {i}: {sc[i].Name}");
            }
        }
    }
}
```

### Ver también

* class [SeriesCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)



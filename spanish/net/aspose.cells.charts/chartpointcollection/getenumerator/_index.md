---
title: "ChartPointCollection.GetEnumerator"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método ChartPointCollection. Devuelve un enumerador para todo ChartPointCollection"
type: docs
url: /es/net/aspose.cells.charts/chartpointcollection/getenumerator/
---
## ChartPointCollection.GetEnumerator method

Devuelve un enumerador para todo [`ChartPointCollection`](../).

```csharp
public IEnumerator GetEnumerator()
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;
    using System.Collections;

    public class ChartPointCollectionMethodGetEnumeratorDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo para el gráfico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Cat1");
            worksheet.Cells["A3"].PutValue("Cat2");
            worksheet.Cells["A4"].PutValue("Cat3");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Agregar un gráfico a la hoja de cálculo
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Establecer origen de datos del Chart
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            try
            {
                // Obtener la colección de puntos de la primera serie
                ChartPointCollection points = chart.NSeries[0].Points;

                // Llame al método GetEnumerator
                IEnumerator enumerator = points.GetEnumerator();

                Console.WriteLine("Iterating through chart points:");
                while (enumerator.MoveNext())
                {
                    ChartPoint point = (ChartPoint)enumerator.Current;
                    Console.WriteLine($"Point value: {point.YValue}");
                }

                Console.WriteLine("Method executed successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetEnumerator method: {ex.Message}");
            }

            // Guardar el resultado
            workbook.Save("MethodGetEnumeratorDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ChartPointCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)



---
title: "ChartPointCollection.RemoveAt"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método de ChartPointCollection. Elimina el punto en el índice de la serie"
type: docs
url: /es/net/aspose.cells.charts/chartpointcollection/removeat/
---
## ChartPointCollection.RemoveAt method

Elimina el punto en el índice de la serie.

```csharp
public void RemoveAt(int index)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | Int32 | El índice del punto. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointCollectionMethodRemoveAtWithInt32Demo
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

            // Añade un gráfico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Establecer rango de datos del gráfico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Obtener la colección de puntos de la primera serie
            ChartPointCollection points = chart.NSeries[0].Points;

            try
            {
                // Mostrar el recuento inicial
                Console.WriteLine($"Initial points count: {points.Count}");

                // Eliminar el punto en el índice 1 (segundo punto)
                points.RemoveAt(1);

                // Mostrar resultado
                Console.WriteLine($"Points count after RemoveAt: {points.Count}");
                Console.WriteLine("Point at index 1 removed successfully.");

                // Guarda el libro de trabajo
                workbook.Save("ChartPointCollectionRemoveAtDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing RemoveAt method: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [ChartPointCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)



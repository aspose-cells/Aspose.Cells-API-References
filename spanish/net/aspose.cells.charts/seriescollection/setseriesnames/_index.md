---
title: "SeriesCollection.SetSeriesNames"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método SeriesCollection. Establece los nombres de todas las series en el gráfico"
type: docs
url: /es/net/aspose.cells.charts/seriescollection/setseriesnames/
---
## SeriesCollection.SetSeriesNames method

Establece los nombres de todas las series en el gráfico.

```csharp
public void SetSeriesNames(int startIndex, string area, bool isVertical)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| startIndex | Int32 | El índice de la primera serie cuyo nombre deseas establecer. |
| área | String | Especifica el área para el nombre de la serie. |
| isVertical | Booleano | &gt;Especifica si se debe trazar la serie a partir de un rango de valores de celdas por fila o por columna. |

### Observaciones

Si el índice de inicio es mayor que la cantidad de series, la función retornará y no hará nada. Si se establecen datos en celdas contiguas, use dos puntos para separarlas. Por ejemplo, $C$2:$C$5. Si se establecen datos en celdas contiguas, use coma para separarlas. Por ejemplo, ($C$2,$D$5).

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class SeriesCollectionMethodSetSeriesNamesWithInt32StringBooleanDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de muestra a las celdas
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["B1"].PutValue("Q1");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(150);
            worksheet.Cells["B4"].PutValue(200);
            worksheet.Cells["C1"].PutValue("Q2");
            worksheet.Cells["C2"].PutValue(120);
            worksheet.Cells["C3"].PutValue(180);
            worksheet.Cells["C4"].PutValue(220);

            // Añade un gráfico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Obtener la colección de series del gráfico
            SeriesCollection seriesCollection = chart.NSeries;

            try
            {
                // Llamar a SetSeriesNames con los parámetros (startIndex: 0, area: "A2:A4", isVertical: true)
                seriesCollection.SetSeriesNames(0, "A2:A4", true);

                // Agregar datos de la serie
                seriesCollection.Add("B2:C4", true);

                Console.WriteLine("SetSeriesNames method executed successfully with parameters (Int32, String, Boolean)");
                Console.WriteLine("Series names set from range A2:A4");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetSeriesNames method: {ex.Message}");
            }

            // Guardar el resultado
            workbook.Save("SeriesCollectionMethodSetSeriesNamesWithInt32StringBooleanDemo.xlsx");
        }
    }
}
```

### Ver también

* class [SeriesCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)



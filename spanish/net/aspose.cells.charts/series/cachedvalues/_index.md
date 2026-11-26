---
title: "Series.CachedValues"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Series. Obtiene los valores en caché de la serie"
type: docs
url: /es/net/aspose.cells.charts/series/cachedvalues/
---
## Series.CachedValues property

Obtiene los valores en caché de la serie

```csharp
[Obsolete("internal use only")]
[EditorBrowsable(EditorBrowsableState.Never)]
public ArrayList CachedValues { get; }
```

### Observaciones

NOTA: Esta propiedad es actualmente solo para uso interno. Será cambiada o eliminada en la próxima versión.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;
    using System.Collections;

    public class SeriesPropertyCachedValuesDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo para el gráfico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue("Banana");

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(15);
            worksheet.Cells["B3"].PutValue(25);
            worksheet.Cells["B4"].PutValue(10);

            // Añade un gráfico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Establecer rango de datos del gráfico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            try
            {
                // Acceder a la primera serie
                Series series = chart.NSeries[0];

                // Mostrar los valores en caché
                ArrayList cachedValues = series.CachedValues;
                Console.WriteLine("CachedValues count: " + cachedValues.Count);

                // Mostrar cada valor en caché
                for (int i = 0; i < cachedValues.Count; i++)
                {
                    Console.WriteLine("Cached Value " + (i + 1) + ": " + cachedValues[i]);
                }

                // Guarda el libro de trabajo
                workbook.Save("CachedValuesDemo.xlsx");
                Console.WriteLine("CachedValues demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)



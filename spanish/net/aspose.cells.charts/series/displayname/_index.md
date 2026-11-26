---
title: "Series.DisplayName"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Series. Obtiene el nombre de la serie que se muestra en el gráfico"
type: docs
url: /es/net/aspose.cells.charts/series/displayname/
---
## Series.DisplayName property

Obtiene el nombre de la serie que se muestra en el gráfico.

```csharp
public string DisplayName { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class SeriesPropertyDisplayNameDemo
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
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);

            // Añade un gráfico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Establecer rango de datos del gráfico
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            try
            {
                // Acceder a la primera serie y mostrar su DisplayName
                Series series = chart.NSeries[0];
                Console.WriteLine("Series DisplayName: " + series.DisplayName);

                // También mostrar la propiedad Name para comparación
                Console.WriteLine("Series Name: " + series.Name);

                // Guarda el libro de trabajo
                workbook.Save("DisplayNameDemo.xlsx");
                Console.WriteLine("DisplayName has been demonstrated successfully.");
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



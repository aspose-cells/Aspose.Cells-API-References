---
title: "ChartPoint.DataLabels"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ChartPoint. Devuelve un objeto DataLabels que representa la etiqueta de datos asociada a este punto del gráfico"
type: docs
url: /es/net/aspose.cells.charts/chartpoint/datalabels/
---
## ChartPoint.DataLabels property

Devuelve un objeto `DataLabels` que representa la etiqueta de datos asociada a este punto del gráfico.

```csharp
public DataLabels DataLabels { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyDataLabelsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregue datos de muestra para el gráfico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Agregar un gráfico de columnas
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Establecer origen de datos del Chart
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            try
            {
                // Acceder al primer punto del gráfico
                ChartPoint point = chart.NSeries[0].Points[0];

                // Obtener la propiedad DataLabels (solo lectura)
                DataLabels dataLabels = point.DataLabels;

                // Mostrar las propiedades de DataLabels
                Console.WriteLine("DataLabels ShowValue: " + dataLabels.ShowValue);
                Console.WriteLine("DataLabels ShowCategoryName: " + dataLabels.ShowCategoryName);
                Console.WriteLine("DataLabels ShowSeriesName: " + dataLabels.ShowSeriesName);
                Console.WriteLine("DataLabels Position: " + dataLabels.Position);

                // Modificar algunas propiedades de DataLabels (ya que DataLabels no es de solo lectura)
                dataLabels.ShowValue = true;
                dataLabels.ShowCategoryName = true;
                dataLabels.Position = LabelPositionType.OutsideEnd;

                // Guardar el resultado
                workbook.Save("ChartPointDataLabelsDemo.xlsx");
                Console.WriteLine("DataLabels demonstration completed successfully.");
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

* class [DataLabels](../../datalabels/)
* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)



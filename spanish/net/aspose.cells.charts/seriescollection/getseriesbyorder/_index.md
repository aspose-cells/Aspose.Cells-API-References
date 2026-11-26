---
title: "SeriesCollection.GetSeriesByOrder"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método SeriesCollection. Obtiene el elemento Series por orden"
type: docs
url: /es/net/aspose.cells.charts/seriescollection/getseriesbyorder/
---
## SeriesCollection.GetSeriesByOrder method

Obtiene el elemento [`Series`](../../series/) por orden.

```csharp
public Series GetSeriesByOrder(int order)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| orden | Int32 | El orden de las series |

### Valor de retorno

El elemento serie

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class SeriesCollectionMethodGetSeriesByOrderWithInt32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de muestra a las celdas
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Q1");
            worksheet.Cells["A3"].PutValue("Q2");
            worksheet.Cells["A4"].PutValue("Q3");
            worksheet.Cells["A5"].PutValue("Q4");
            
            worksheet.Cells["B1"].PutValue("Series 1");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["B4"].PutValue(300);
            worksheet.Cells["B5"].PutValue(400);
            
            worksheet.Cells["C1"].PutValue("Series 2");
            worksheet.Cells["C2"].PutValue(150);
            worksheet.Cells["C3"].PutValue(250);
            worksheet.Cells["C4"].PutValue(350);
            worksheet.Cells["C5"].PutValue(450);

            // Crear un gráfico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Establecer rango de datos del gráfico
            chart.NSeries.Add("B2:B5", true);
            chart.NSeries.Add("C2:C5", true);
            chart.NSeries.CategoryData = "A2:A5";

            try
            {
                // Obtener la primera serie (orden = 0)
                Series series = chart.NSeries.GetSeriesByOrder(0);
                
                if (series != null)
                {
                    // Modificar las propiedades de la serie
                    series.Name = "Modified Series 1";
                    series.Shadow = true;
                    
                    Console.WriteLine("Successfully retrieved and modified series with order 0");
                    Console.WriteLine($"Series Name: {series.Name}");
                    Console.WriteLine($"Shadow Enabled: {series.Shadow}");
                }
                
                // Guarda el libro de trabajo
                workbook.Save("SeriesCollectionMethodGetSeriesByOrderDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetSeriesByOrder method: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [Series](../../series/)
* class [SeriesCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)



---
title: "SeriesCollection.RemoveAt"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método SeriesCollection. Elimina una serie en el índice específico"
type: docs
url: /es/net/aspose.cells.charts/seriescollection/removeat/
---
## SeriesCollection.RemoveAt method

Eliminar una serie en el índice específico.

```csharp
public void RemoveAt(int index)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | Int32 | El índice. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class SeriesCollectionMethodRemoveAtWithInt32Demo
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
            worksheet.Cells["B1"].PutValue("Series1");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["B4"].PutValue(300);
            worksheet.Cells["C1"].PutValue("Series2");
            worksheet.Cells["C2"].PutValue(150);
            worksheet.Cells["C3"].PutValue(250);
            worksheet.Cells["C4"].PutValue(350);

            // Añade un gráfico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Establecer rango de datos del gráfico
            chart.NSeries.Add("B1:B4", true);
            chart.NSeries.Add("C1:C4", true);
            chart.NSeries.CategoryData = "A2:A4";

            try
            {
                // Llamar a RemoveAt para eliminar la primera serie (índice 0)
                chart.NSeries.RemoveAt(0);
                
                Console.WriteLine("Series at index 0 removed successfully");
                
                // Verificar el recuento de series restantes
                Console.WriteLine($"Remaining series count: {chart.NSeries.Count}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing RemoveAt method: {ex.Message}");
            }
            
            // Guardar el resultado
            workbook.Save("SeriesCollectionMethodRemoveAtWithInt32Demo.xlsx");
        }
    }
}
```

### Ver también

* class [SeriesCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)



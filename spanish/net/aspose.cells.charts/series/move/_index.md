---
title: "Series.Move"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Series. Mueve la serie hacia arriba o hacia abajo"
type: docs
url: /es/net/aspose.cells.charts/series/move/
---
## Series.Move method

Mueve la serie hacia arriba o hacia abajo.

```csharp
public void Move(int count)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| contar | Int32 | El número de movimientos hacia arriba o hacia abajo. Mueve la serie hacia arriba si es menor que cero; mueve la serie hacia abajo si es mayor que cero. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class SeriesMethodMoveWithInt32Demo
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
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Agregar series al gráfico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // Obtener la primera serie
            Series series = chart.NSeries[0];
            
            try
            {
                // Llame al método Move con el parámetro Int32
                series.Move(1);
                
                Console.WriteLine("Series moved successfully by 1 position");
                
                // Muestre el efecto cambiando el nombre de la serie
                series.Name = "Moved Series";
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Move method: {ex.Message}");
            }
            
            // Guardar el resultado
            workbook.Save("SeriesMethodMoveWithInt32Demo.xlsx");
        }
    }
}
```

### Ver también

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)



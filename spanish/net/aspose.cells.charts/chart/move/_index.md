---
title: "Chart.Move"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método del gráfico. Mueve el gráfico a una ubicación especificada"
type: docs
url: /es/net/aspose.cells.charts/chart/move/
---
## Chart.Move method

Mueve el gráfico a una ubicación especificada.

```csharp
public void Move(int topRow, int leftColumn, int bottomRow, int rightColumn)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| leftColumn | Int32 | Índice de columna superior izquierda. |
| topRow | Int32 | Índice de fila superior izquierda. |
| rightColumn | Int32 | Índice de columna inferior derecha |
| bottomRow | Int32 | Índice de fila inferior derecha |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartMethodMoveWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregue datos de muestra para el gráfico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Fruits");
            worksheet.Cells["A3"].PutValue("Vegetables");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(50);
            worksheet.Cells["B3"].PutValue(30);

            // Agregar un gráfico a la hoja de cálculo
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Establecer origen de datos del Chart
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            try
            {
                // Posición original del gráfico
                Console.WriteLine($"Original position - topRow: {chart.ChartObject.UpperLeftRow}, leftColumn: {chart.ChartObject.UpperLeftColumn}");

                // Mover el gráfico a una nueva posición (filas 10-20, columnas 2-8)
                chart.Move(10, 2, 20, 8);

                // Mostrar nueva posición
                Console.WriteLine($"New position - topRow: {chart.ChartObject.UpperLeftRow}, leftColumn: {chart.ChartObject.UpperLeftColumn}");

                // Guarda el libro de trabajo
                workbook.Save("ChartMoveDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Move method: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)



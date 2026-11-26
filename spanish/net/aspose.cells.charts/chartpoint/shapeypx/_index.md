---
title: "ChartPoint.ShapeYPx"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ChartPoint. Obtiene la coordenada y de la esquina superior izquierda en unidades de píxeles después de llamar al método Chart.Calculate"
type: docs
url: /es/net/aspose.cells.charts/chartpoint/shapeypx/
---
## ChartPoint.ShapeYPx property

Obtiene la coordenada y de la esquina superior izquierda en unidades de píxeles después de llamar al método Chart.Calculate().

```csharp
public int ShapeYPx { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyShapeYPxDemo
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

            // Agregar un gráfico de columnas
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Calcular el gráfico para obtener las posiciones de las formas
            chart.Calculate();

            // Obtener el primer punto en la primera serie
            ChartPoint point = chart.NSeries[0].Points[0];

            // Mostrar la posición Y actual en píxeles
            Console.WriteLine("Current ShapeYPx value: " + point.ShapeYPx);

            // Nota: ShapeYPx es de solo lectura, por lo que no podemos establecerlo directamente
            // Para cambiar la posición, necesitamos modificar el tamaño/posición del gráfico o los datos

            // Demostrar el efecto cambiando la posición del gráfico, lo que afectará las posiciones de los puntos
            chart.Move(2, 3, 17, 11); // Move chart to row 2, column 3
            chart.Calculate(); // Recalculate to update positions

            // Mostrar la nueva posición Y después del movimiento del gráfico
            Console.WriteLine("New ShapeYPx value after chart movement: " + point.ShapeYPx);

            // Guardar el resultado
            workbook.Save("ChartPointShapeYPxDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)



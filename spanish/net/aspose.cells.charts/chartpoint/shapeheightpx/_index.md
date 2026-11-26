---
title: "ChartPoint.ShapeHeightPx"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ChartPoint. Obtiene la altura en unidades de píxeles después de llamar al método Chart.Calculate"
type: docs
url: /es/net/aspose.cells.charts/chartpoint/shapeheightpx/
---
## ChartPoint.ShapeHeightPx property

Obtiene la altura en unidades de píxeles después de llamar al método Chart.Calculate().

```csharp
public int ShapeHeightPx { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyShapeHeightPxDemo
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
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Calcule el gráfico para obtener las dimensiones de la forma
            chart.Calculate();

            // Obtén el primer punto del gráfico de la primera serie
            ChartPoint chartPoint = chart.NSeries[0].Points[0];

            // Muestre la altura actual de la forma del punto del gráfico en píxeles
            Console.WriteLine("Current ShapeHeightPx value: " + chartPoint.ShapeHeightPx);

            // Nota: ShapeHeightPx es de solo lectura, por lo que no podemos establecerlo directamente
            // Para cambiar la altura, necesitaríamos modificar el tamaño del gráfico o los valores de datos
            // y recalcular el gráfico

            // Cambie el valor de datos que afectará al tamaño del punto del gráfico
            worksheet.Cells["B2"].PutValue(50);
            chart.Calculate();

            // Muestre la nueva altura después de cambiar los datos
            Console.WriteLine("New ShapeHeightPx value after data change: " + chartPoint.ShapeHeightPx);

            // Guarda el libro de trabajo
            workbook.Save("ChartPointShapeHeightPxDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)



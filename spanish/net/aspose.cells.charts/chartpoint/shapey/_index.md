---
title: "ChartPoint.ShapeY"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ChartPoint. Obtiene la coordenada y de la esquina superior izquierda en unidades de 1/4000 de la altura del gráfico después de llamar al método Chart.Calculate"
type: docs
url: /es/net/aspose.cells.charts/chartpoint/shapey/
---
## ChartPoint.ShapeY property

Obtiene la coordenada y de la esquina superior izquierda en unidades de 1/4000 de la altura del gráfico después de llamar al método Chart.Calculate().

```csharp
public int ShapeY { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyShapeYDemo
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

            // Calcular el gráfico para obtener las posiciones de las formas
            chart.Calculate();

            // Obtenga el primer punto de la primera serie
            ChartPoint point = chart.NSeries[0].Points[0];

            // Muestra el valor actual de ShapeY (1/4000 de la altura del gráfico)
            Console.WriteLine("Current ShapeY value: " + point.ShapeY);

            // Nota: ShapeY es de solo lectura, por lo que no podemos establecerlo directamente
            // Para cambiar la posición, necesitaríamos modificar los datos subyacentes o las propiedades del gráfico

            // Demuestra cómo ShapeY se relaciona con la posición real
            Console.WriteLine("ShapeY in pixels: " + point.ShapeYPx);
            Console.WriteLine("Chart height in pixels: " + (point.ShapeYPx * 4000 / point.ShapeY));

            // Guardar el resultado
            workbook.Save("ChartPointPropertyShapeYDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)



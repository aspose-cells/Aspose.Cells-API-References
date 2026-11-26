---
title: "ChartPoint.ShapeHeight"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ChartPoint. Obtiene la altura en unidades de 1/4000 de la altura del gráfico después de llamar al método Chart.Calculate"
type: docs
url: /es/net/aspose.cells.charts/chartpoint/shapeheight/
---
## ChartPoint.ShapeHeight property

Obtiene la altura en unidades de 1/4000 de la altura del gráfico después de llamar al método Chart.Calculate().

```csharp
public int ShapeHeight { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyShapeHeightDemo
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

            // Calcule el gráfico para asegurar que las propiedades de forma estén disponibles
            chart.Calculate();

            // Obtenga el primer punto de la primera serie
            ChartPoint point = chart.NSeries[0].Points[0];

            // Muestre el valor actual de ShapeHeight (en 1/4000 de la altura del gráfico)
            Console.WriteLine("Current ShapeHeight value: " + point.ShapeHeight);

            // Nota: ShapeHeight es de solo lectura, por lo que no podemos establecerlo directamente
            // Para cambiar la altura, necesitamos modificar el tamaño del gráfico u otras propiedades

            // Demuestre el efecto cambiando la altura del gráfico
            Console.WriteLine("Original chart height: " + chart.ChartObject.Height);
            chart.ChartObject.Height = 400;
            chart.Calculate(); // Recalculate to update shape properties

            // Muestre el nuevo valor de ShapeHeight después de cambiar la altura del gráfico
            Console.WriteLine("New ShapeHeight value after chart resize: " + point.ShapeHeight);

            // Guardar el resultado
            workbook.Save("ChartPointPropertyShapeHeightDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)



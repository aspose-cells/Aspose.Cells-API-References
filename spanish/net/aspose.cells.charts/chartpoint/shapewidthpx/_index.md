---
title: "ChartPoint.ShapeWidthPx"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ChartPoint. Obtiene el ancho en unidades de píxeles después de llamar al método Chart.Calculate"
type: docs
url: /es/net/aspose.cells.charts/chartpoint/shapewidthpx/
---
## ChartPoint.ShapeWidthPx property

Obtiene el ancho en unidades de píxeles después de llamar al método Chart.Calculate().

```csharp
public int ShapeWidthPx { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyShapeWidthPxDemo
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

            // Calcule el gráfico para asegurar que las propiedades de forma estén disponibles
            chart.Calculate();

            // Obtener el primer punto del gráfico de la primera serie
            ChartPoint point = chart.NSeries[0].Points[0];

            // Mostrar el ancho actual de la forma del punto del gráfico en píxeles
            Console.WriteLine("Current ShapeWidthPx value: " + point.ShapeWidthPx);

            // Nota: ShapeWidthPx es de solo lectura, por lo que no podemos establecerlo directamente
            // Para cambiar el ancho, necesitamos modificar el tamaño del gráfico u otras propiedades
            // eso afectaría el ancho del punto durante el siguiente Calculate()

            // Cambiar el ancho del gráfico para demostrar cómo afecta a ShapeWidthPx
            chart.ChartObject.Width = 1000;
            chart.Calculate();

            // Mostrar el nuevo ancho después de redimensionar el gráfico
            Console.WriteLine("New ShapeWidthPx value after chart resize: " + point.ShapeWidthPx);

            // Guardar el resultado
            workbook.Save("ChartPointPropertyShapeWidthPxDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)



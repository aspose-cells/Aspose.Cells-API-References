---
title: "ChartPoint.ArcStartPointYPx"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de ChartPoint. Obtiene la coordenada y del punto de inicio para la sección del pastel después de llamar al método Chart.Calculate. Se aplica a gráficos de pastel y rosquilla."
type: docs
url: /es/net/aspose.cells.charts/chartpoint/arcstartpointypx/
---
## ChartPoint.ArcStartPointYPx property

Obtiene la coordenada y del punto inicial de la sección de pastel después de llamar al método Chart.Calculate(). Se aplica a los gráficos de pastel y dona.

```csharp
public float ArcStartPointYPx { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyArcStartPointYPxDemo
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

            // Agregar un gráfico de pastel
            int chartIndex = worksheet.Charts.Add(ChartType.Pie, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Calcule el gráfico para obtener las posiciones de las formas
            chart.Calculate();

            // Obtener el primer punto del gráfico
            ChartPoint point = chart.NSeries[0].Points[0];

            // Mostrar el valor actual de ArcStartPointYPx
            Console.WriteLine("Current ArcStartPointYPx value: " + point.ArcStartPointYPx);

            // Nota: ArcStartPointYPx es de solo lectura, por lo que no podemos establecerlo directamente
            // En su lugar, demostraremos cómo al cambiar otras propiedades afecta a ArcStartPointYPx

            // Cambie el valor de explosión para modificar la posición de la porción del pastel
            point.Explosion = 20;

            // Recalcule el gráfico para actualizar las posiciones
            chart.Calculate();

            // Muestre el nuevo valor de ArcStartPointYPx después de cambiar la explosión
            Console.WriteLine("New ArcStartPointYPx after explosion change: " + point.ArcStartPointYPx);

            // Guarda el libro de trabajo
            workbook.Save("ChartPointPropertyArcStartPointYPxDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)



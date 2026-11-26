---
title: "ChartPoint.ArcStartPointXPx"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de ChartPoint. Obtiene la coordenada x del punto de inicio para la sección de pastel después de llamar al método Chart.Calculate. Se aplica a gráficos de pastel y rosquilla."
type: docs
url: /es/net/aspose.cells.charts/chartpoint/arcstartpointxpx/
---
## ChartPoint.ArcStartPointXPx property

Obtiene la coordenada x del punto inicial de la sección de pastel después de llamar al método Chart.Calculate(). Se aplica a los gráficos de pastel y dona.

```csharp
public float ArcStartPointXPx { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyArcStartPointXPxDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo para el gráfico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Agregar un gráfico de pastel
            int chartIndex = worksheet.Charts.Add(ChartType.Pie, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Establecer rango de datos del gráfico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Calcular el gráfico para asegurar que las propiedades estén pobladas
            chart.Calculate();

            // Obtener el primer punto del gráfico
            ChartPoint point = chart.NSeries[0].Points[0];

            // Mostrar el valor de ArcStartPointXPx
            Console.WriteLine("ArcStartPointXPx for first point: " + point.ArcStartPointXPx);

            // Nota: ArcStartPointXPx es de solo lectura, por lo que no podemos establecerlo directamente
            // En su lugar, podemos demostrar cómo cambia cuando modificamos otras propiedades

            // Cambiar el valor de explosión que afecta la posición de la porción del pastel
            point.Explosion = 20;
            chart.Calculate(); // Recalculate to update properties

            // Mostrar el nuevo valor de ArcStartPointXPx después de cambiar la explosión
            Console.WriteLine("ArcStartPointXPx after explosion: " + point.ArcStartPointXPx);

            // Guarda el libro de trabajo
            workbook.Save("ChartPointPropertyArcStartPointXPxDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)



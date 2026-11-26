---
title: "ChartPoint.ArcEndPointXPx"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ChartPoint. Obtiene la coordenada x del punto final de la sección de pastel después de llamar al método Chart.Calculate. Se aplica a gráficos Pie y Doughnut."
type: docs
url: /es/net/aspose.cells.charts/chartpoint/arcendpointxpx/
---
## ChartPoint.ArcEndPointXPx property

Obtiene la coordenada x del punto final de la sección de pastel después de llamar al método Chart.Calculate(). Se aplica a los gráficos de pastel y dona.

```csharp
public float ArcEndPointXPx { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyArcEndPointXPxDemo
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
            worksheet.Cells["B2"].PutValue(50);
            worksheet.Cells["B3"].PutValue(30);
            worksheet.Cells["B4"].PutValue(20);

            // Agregar un gráfico de pastel
            int chartIndex = worksheet.Charts.Add(ChartType.Pie, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Calcular el gráfico para asegurar que las propiedades estén pobladas
            chart.Calculate();

            // Obtener el primer punto del gráfico
            ChartPoint point = chart.NSeries[0].Points[0];

            // Mostrar el valor de ArcEndPointXPx
            Console.WriteLine("ArcEndPointXPx: " + point.ArcEndPointXPx);

            // Nota: ArcEndPointXPx es de solo lectura, por lo que no podemos establecerlo directamente
            // Para cambiar el punto final, necesitamos modificar los datos del gráfico o las propiedades que afectan la porción del pastel
            
            // Ejemplo de cómo cambiar los datos afecta a ArcEndPointXPx
            worksheet.Cells["B2"].PutValue(60); // Increase Apple's value
            chart.Calculate(); // Recalculate chart

            // Mostrar el nuevo valor de ArcEndPointXPx después del cambio de datos
            Console.WriteLine("New ArcEndPointXPx after data change: " + point.ArcEndPointXPx);

            // Guarda el libro de trabajo
            workbook.Save("ChartPointPropertyArcEndPointXPxDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)



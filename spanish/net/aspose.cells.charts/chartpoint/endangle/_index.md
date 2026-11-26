---
title: "ChartPoint.EndAngle"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de ChartPoint. Obtiene el ángulo final de la sección del pastel medido en grados en sentido horario desde el eje x después de llamar al método Chart.Calculate. Se aplica a gráficos de pastel."
type: docs
url: /es/net/aspose.cells.charts/chartpoint/endangle/
---
## ChartPoint.EndAngle property

Obtiene el ángulo final de la sección de pastel, medido en grados en sentido horario desde el eje x después de llamar al método Chart.Calculate(). Se aplica al gráfico de pastel.

```csharp
public float EndAngle { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyEndAngleDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de muestra para el gráfico de pastel
            worksheet.Cells["A1"].PutValue("Fruit");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["B1"].PutValue("Quantity");
            worksheet.Cells["B2"].PutValue(50);
            worksheet.Cells["B3"].PutValue(30);
            worksheet.Cells["B4"].PutValue(20);

            // Agregar un gráfico de pastel
            int chartIndex = worksheet.Charts.Add(ChartType.Pie, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Calcular el gráfico para asegurar que las propiedades estén pobladas
            chart.Calculate();

            // Obtener el primer punto del gráfico (porción de Manzana)
            ChartPoint point = chart.NSeries[0].Points[0];

            // Mostrar el valor actual de EndAngle
            Console.WriteLine("Current EndAngle value: " + point.EndAngle);

            // Nota: EndAngle es de solo lectura, por lo que no podemos establecerlo directamente
            // En su lugar, demostraremos cómo se relaciona con la porción del pastel

            // Explotar el punto para ver cómo afecta a los ángulos
            point.Explosion = 20;
            chart.Calculate(); // Recalculate to update angles

            // Mostrar el nuevo EndAngle después de la explosión
            Console.WriteLine("EndAngle after explosion: " + point.EndAngle);

            // Guarda el libro de trabajo
            workbook.Save("ChartPointEndAngleDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)



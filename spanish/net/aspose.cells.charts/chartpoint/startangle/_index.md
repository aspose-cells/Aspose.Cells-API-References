---
title: "ChartPoint.StartAngle"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ChartPoint. Obtiene el ángulo inicial para la sección de pastel medido en grados en sentido horario desde el eje x después de llamar al método Chart.Calculate. Se aplica al gráfico de pastel"
type: docs
url: /es/net/aspose.cells.charts/chartpoint/startangle/
---
## ChartPoint.StartAngle property

Obtiene el ángulo inicial para la sección de pastel, medido en grados en sentido horario desde el eje x después de llamar al método Chart.Calculate(). Se aplica al gráfico de pastel.

```csharp
public float StartAngle { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyStartAngleDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregue datos de muestra para el gráfico
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
            
            // Establecer rango de datos del gráfico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Calcular el gráfico para asegurar que las propiedades estén pobladas
            chart.Calculate();

            // Obtener el primer punto del gráfico
            ChartPoint point = chart.NSeries[0].Points[0];

            // Mostrar el valor de StartAngle
            Console.WriteLine("StartAngle of first pie slice: " + point.StartAngle);

            // Nota: StartAngle es de solo lectura, por lo que no podemos establecerlo directamente
            // Para cambiar el ángulo inicial, necesitamos rotar todo el gráfico de pastel
            chart.NSeries[0].FirstSliceAngle = 90; // Rotate pie chart by 90 degrees

            // Recalcular para actualizar los ángulos
            chart.Calculate();

            // Mostrar el nuevo valor de StartAngle después de la rotación
            Console.WriteLine("StartAngle after rotation: " + point.StartAngle);

            // Guarda el libro de trabajo
            workbook.Save("ChartPointPropertyStartAngleDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)



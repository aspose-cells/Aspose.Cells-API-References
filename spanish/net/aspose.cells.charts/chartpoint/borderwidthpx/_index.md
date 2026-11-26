---
title: "ChartPoint.BorderWidthPx"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ChartPoint. Obtiene el ancho del borde en unidades de píxeles después de llamar al método Chart.Calculate"
type: docs
url: /es/net/aspose.cells.charts/chartpoint/borderwidthpx/
---
## ChartPoint.BorderWidthPx property

Obtiene el ancho del borde en unidades de píxeles después de llamar al método Chart.Calculate().

```csharp
public int BorderWidthPx { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;

    public class ChartPointPropertyBorderWidthPxDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregue datos de muestra para el gráfico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Q1");
            worksheet.Cells["A3"].PutValue("Q2");
            worksheet.Cells["A4"].PutValue("Q3");
            worksheet.Cells["A5"].PutValue("Q4");
            
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1200);
            worksheet.Cells["B3"].PutValue(1500);
            worksheet.Cells["B4"].PutValue(1800);
            worksheet.Cells["B5"].PutValue(2100);

            // Agregar un gráfico y establecer su rango de datos
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B5", true);
            chart.NSeries.CategoryData = "A2:A5";

            // Calcular el gráfico para asegurar que las propiedades estén pobladas
            chart.Calculate();

            // Obtener el primer punto del gráfico en la primera serie
            ChartPoint point = chart.NSeries[0].Points[0];

            // Mostrar el ancho de borde actual
            Console.WriteLine("Current BorderWidthPx value: " + point.BorderWidthPx);

            // Nota: BorderWidthPx es de solo lectura, por lo que no podemos establecerlo directamente
            // En su lugar, podemos modificar el borde a través de la propiedad Border
            if (point.Border != null)
            {
                // Cambiar el ancho del borde estableciendo el peso mediante el enum WeightType
                point.Border.Weight = WeightType.MediumLine; // Medium weight border
            }

            // Recalcular para actualizar el valor de BorderWidthPx
            chart.Calculate();

            // Mostrar el nuevo ancho de borde en píxeles
            Console.WriteLine("New BorderWidthPx value after modification: " + point.BorderWidthPx);

            // Guarda el libro de trabajo
            workbook.Save("ChartPointPropertyBorderWidthPxDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)



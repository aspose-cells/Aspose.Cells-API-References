---
title: "ChartPoint.YValueType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ChartPoint. Obtiene el tipo de valor Y del punto del gráfico"
type: docs
url: /es/net/aspose.cells.charts/chartpoint/yvaluetype/
---
## ChartPoint.YValueType property

Obtiene el tipo de valor Y del punto del gráfico.

```csharp
public CellValueType YValueType { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyYValueTypeDemo
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

            // Agregar un gráfico a la hoja de cálculo
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Establecer rango de datos del gráfico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Obtener el primer punto del gráfico en la primera serie
            ChartPoint chartPoint = chart.NSeries[0].Points[0];

            // Mostrar el YValueType actual
            Console.WriteLine("Current YValueType: " + chartPoint.YValueType);

            // Mostrar el YValue antes del cambio
            Console.WriteLine("Current YValue: " + chartPoint.YValue);

            // Cambiar el YValue a un tipo diferente (string para demostrar el cambio de tipo)
            chartPoint.YValue = "15"; // This will change the YValueType to IsString

            // Mostrar el YValueType después del cambio
            Console.WriteLine("New YValueType: " + chartPoint.YValueType);
            Console.WriteLine("New YValue: " + chartPoint.YValue);

            // Guarda el libro de trabajo
            workbook.Save("ChartPointPropertyYValueTypeDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [CellValueType](../../../aspose.cells/cellvaluetype/)
* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)



---
title: "ChartPoint.XValueType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ChartPoint. Obtiene el tipo de valor X del punto del gráfico"
type: docs
url: /es/net/aspose.cells.charts/chartpoint/xvaluetype/
---
## ChartPoint.XValueType property

Obtiene el tipo de valor X del punto del gráfico.

```csharp
public CellValueType XValueType { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyXValueTypeDemo
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

            // Añade un gráfico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Establecer rango de datos del gráfico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Obtener el primer punto del gráfico
            ChartPoint point = chart.NSeries[0].Points[0];

            // Mostrar el XValueType actual
            Console.WriteLine("Current XValueType: " + point.XValueType);

            // Establecer un nuevo XValue (esto actualizará automáticamente XValueType)
            point.XValue = DateTime.Now; // Changing to DateTime type
            Console.WriteLine("After setting DateTime value, XValueType: " + point.XValueType);

            point.XValue = "New Category"; // Changing to String type
            Console.WriteLine("After setting String value, XValueType: " + point.XValueType);

            point.XValue = 123.45; // Changing to Numeric type
            Console.WriteLine("After setting Numeric value, XValueType: " + point.XValueType);

            // Guarda el libro de trabajo
            workbook.Save("ChartPointXValueTypeDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [CellValueType](../../../aspose.cells/cellvaluetype/)
* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)



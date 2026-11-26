---
title: "Chart.ActualChartSize"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Chart. Obtiene el tamaño real del gráfico en unidades de píxeles"
type: docs
url: /es/net/aspose.cells.charts/chart/actualchartsize/
---
## Chart.ActualChartSize property

Obtiene el tamaño real del gráfico en unidades de píxeles.

```csharp
[Obsolete("Use Chart.GetActualSize() method instead.")]
public Size ActualChartSize { get; }
```

### Observaciones

NOTA: Este miembro está ahora obsoleto. En su lugar, por favor use el método Chart.GetActualSize(). Esta propiedad será eliminada 12 meses después desde julio de 2022. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class ChartPropertyActualChartSizeDemo
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

            // Añade un gráfico
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 10);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B4", true);

            // Calcular el gráfico para asegurar que las propiedades estén pobladas
            chart.Calculate();

            // Demostrar el uso de ActualChartSize
            Console.WriteLine($"Actual Chart Size - Width: {chart.ActualChartSize.Width}, Height: {chart.ActualChartSize.Height}");

            // Agregar una forma cuyo tamaño se basa en ActualChartSize
            Shape shape = chart.Shapes.AddShapeInChartByScale(
                MsoDrawingType.Rectangle,
                PlacementType.Move,
                0.5,  // x position (relative)
                0.5,  // y position (relative)
                0.5 + (0.1 * chart.ActualChartSize.Height / chart.ActualChartSize.Width),  // width adjusted by aspect ratio
                0.6   // height
            );
            shape.Fill.SolidFill.Color = Color.Blue;

            // Guarda el libro de trabajo
            workbook.Save("ChartWithActualSizeDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)



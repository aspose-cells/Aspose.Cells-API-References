---
title: "Title.Y"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Title. Obtiene o establece la coordenada y de la esquina superior izquierda en unidades de 1/4000 del área del gráfico"
type: docs
url: /es/net/aspose.cells.charts/title/y/
---
## Title.Y property

Obtiene o establece la coordenada y de la esquina superior izquierda en unidades de 1/4000 del área del gráfico.

```csharp
[Obsolete("Use Title.YRatioToChart property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public override int Y { get; set; }
```

### Observaciones

NOTA: Este miembro está ahora obsoleto. Por favor, use la propiedad Title.YRatioToChart, en su lugar. Y = YRatioToChart * 4000; Esta propiedad será eliminada 12 meses después a partir de febrero de 2025. Aspose se disculpa por cualquier inconveniente que pueda haber experimentado.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class TitlePropertyYDemo
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
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Establecer rango de datos del gráfico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Establecer título del gráfico
            chart.Title.Text = "Sample Chart";
            chart.Title.Y = 1000; // Demonstrating Y property - position in 1/4000 units
            
            // Calcule el gráfico para asegurar que el diseño se actualice
            chart.Calculate();

            // Agregue una forma alineada con la posición Y del título
            Shape shape = chart.Shapes.AddShapeInChart(MsoDrawingType.Rectangle, PlacementType.Move,
                2000, 
                chart.Title.Y, // Using the title's Y property
                3000, 
                chart.Title.Y + 500);
            shape.Fill.SolidFill.Color = Color.Blue;

            // Guarda el libro de trabajo
            workbook.Save("TitlePropertyYDemo_Output.xlsx");
        }
    }
}
```

### Ver también

* class [Title](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)



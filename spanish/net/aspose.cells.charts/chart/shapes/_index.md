---
title: "Chart.Shapes"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Chart. Devuelve todas las formas de dibujo en este gráfico"
type: docs
url: /es/net/aspose.cells.charts/chart/shapes/
---
## Chart.Shapes property

Devuelve todas las formas de dibujo en este gráfico.

```csharp
public ShapeCollection Shapes { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ChartPropertyShapesDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo para el gráfico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B4"].PutValue(30);

            // Agregar un gráfico a la hoja de cálculo
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Establecer origen de datos del Chart
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Agregar una forma al gráfico
            Aspose.Cells.Drawing.Shape shape = chart.Shapes.AddShape(MsoDrawingType.TextBox, 1000, 1000, 2000, 1000, 0, 0);
            shape.Text = "Sample Shape";
            
            // Modificar propiedades de la forma
            shape.LeftInShape = 4000 - shape.WidthInShape;
            shape.TopInShape = 4000 - shape.HeightInShape;
            
            // Guarda el libro de trabajo
            workbook.Save("ChartPropertyShapesDemo_out.xlsx");
        }
    }
}
```

### Ver también

* class [ShapeCollection](../../../aspose.cells.drawing/shapecollection/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)



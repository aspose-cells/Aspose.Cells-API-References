---
title: "SolidFill.Transparency"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad SolidFill. Devuelve o establece el grado de transparencia del área como un valor de 0.0 opaco a 1.0 transparente"
type: docs
url: /es/net/aspose.cells.drawing/solidfill/transparency/
---
## SolidFill.Transparency property

Devuelve o establece el grado de transparencia del área como un valor de 0.0 (opaco) a 1.0 (claro).

```csharp
public double Transparency { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class SolidFillPropertyTransparencyDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un gráfico de ejemplo
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Agregue datos de muestra para el gráfico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            chart.Calculate();

            // Agregar una forma para demostrar la transparencia
            Shape shape = chart.Shapes.AddShapeInChart(MsoDrawingType.Rectangle, PlacementType.FreeFloating, 
                1000, 1000, 2000, 2000);
            
            // Establezca un relleno sólido con transparencia
            shape.Fill.SolidFill.Color = Color.Blue;
            shape.Fill.SolidFill.Transparency = 0.5; // 50% transparent

            // Agregue otra forma para comparación (totalmente opaca)
            Shape shape2 = chart.Shapes.AddShapeInChart(MsoDrawingType.Rectangle, PlacementType.FreeFloating, 
                3000, 1000, 2000, 2000);
            shape2.Fill.SolidFill.Color = Color.Blue;
            shape2.Fill.SolidFill.Transparency = 0; // 0% transparent (fully opaque)

            // Guarda el libro de trabajo
            workbook.Save("SolidFillTransparencyDemo.xlsx");
        }
    }
}
```

### Ver también

* class [SolidFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)



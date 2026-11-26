---
title: "Line.Color"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Line. Representa el color de la línea"
type: docs
url: /es/net/aspose.cells.drawing/line/color/
---
## Line.Color property

Representa el color de la línea.

```csharp
public Color Color { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class LinePropertyColorDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo para el gráfico
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["A4"].PutValue("C");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["B3"].PutValue(20);
            sheet.Cells["B4"].PutValue(30);

            // Añade un gráfico
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = sheet.Charts[chartIndex];
            
            // Establecer rango de datos del gráfico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Establecer colores de líneas de eje
            chart.CategoryAxis.AxisLine.Color = Color.BlueViolet;
            chart.ValueAxis.AxisLine.Color = Color.BlueViolet;
            
            // Establecer color de fuente del título del eje
            chart.CategoryAxis.Title.Text = "Categories";
            chart.CategoryAxis.Title.Font.Color = Color.BlueViolet;

            // Guarda el libro de trabajo
            workbook.Save("LinePropertyColorDemo_out.xlsx");
        }
    }
}
```

### Ver también

* class [Line](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)



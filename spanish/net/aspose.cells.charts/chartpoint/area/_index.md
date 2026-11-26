---
title: "ChartPoint.Area"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ChartPoint. Obtiene el área"
type: docs
url: /es/net/aspose.cells.charts/chartpoint/area/
---
## ChartPoint.Area property

Obtiene el ` area`.

```csharp
public Area Area { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ChartPointPropertyAreaDemo
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
            sheet.Cells["A5"].PutValue("D");
            
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["B3"].PutValue(20);
            sheet.Cells["B4"].PutValue(30);
            sheet.Cells["B5"].PutValue(40);

            // Añade un gráfico
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = sheet.Charts[chartIndex];
            
            // Establecer rango de datos del gráfico
            chart.NSeries.Add("B2:B5", true);
            chart.NSeries.CategoryData = "A2:A5";

            // Acceder al primer punto de la primera serie y establecer propiedades de área
            Aspose.Cells.Charts.ChartPoint point = chart.NSeries[0].Points[0];
            point.Area.ForegroundColor = System.Drawing.Color.Red;
            point.Area.FillFormat.Texture = TextureType.Granite;
            point.Area.Formatting = FormattingType.Custom;

            // Guarda el libro de trabajo
            workbook.Save("ChartPointAreaDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Area](../../../aspose.cells.drawing/area/)
* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)



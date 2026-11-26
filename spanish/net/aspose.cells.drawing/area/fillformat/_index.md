---
title: "Area.FillFormat"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Area. Representa un objeto FillFormat que contiene propiedades de formato de relleno para el gráfico o forma especificados"
type: docs
url: /es/net/aspose.cells.drawing/area/fillformat/
---
## Area.FillFormat property

Representa un objeto `FillFormat` que contiene propiedades de formato de relleno para el gráfico o forma especificados.

```csharp
public FillFormat FillFormat { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class AreaPropertyFillFormatDemo
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

            // Obtener el tercer punto de la primera serie
            ChartPoint point = chart.NSeries[0].Points[2];
            
            // Establecer propiedades de formato de relleno
            point.Area.FillFormat.Pattern = FillPattern.DashedHorizontal;
            point.Area.FillFormat.SetTwoColorGradient(Color.Blue, Color.LightBlue, GradientStyleType.Horizontal, 2);

            // Guarda el libro de trabajo
            workbook.Save("FillFormatDemo.xlsx");
        }
    }
}
```

### Ver también

* class [FillFormat](../../fillformat/)
* class [Area](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)



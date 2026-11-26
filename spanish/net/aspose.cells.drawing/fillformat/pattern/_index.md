---
title: "FillFormat.Pattern"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad FillFormat. Representa un patrón de visualización de áreas"
type: docs
url: /es/net/aspose.cells.drawing/fillformat/pattern/
---
## FillFormat.Pattern property

Representa el patrón de visualización de un área.

```csharp
public FillPattern Pattern { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class FillFormatPropertyPatternDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            sheet.Cells["A1"].PutValue(50);
            sheet.Cells["A2"].PutValue(100);
            sheet.Cells["A3"].PutValue(150);

            // Añade un gráfico
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = sheet.Charts[chartIndex];
            
            // Establecer rango de datos del gráfico
            chart.NSeries.Add("A1:A3", true);

            // Acceder a la primera serie y su primer punto
            ChartPoint point = chart.NSeries[0].Points[0];
            
            // Establecer el patrón de relleno para el área del punto
            point.Area.FillFormat.Pattern = FillPattern.DottedGrid;
            
            // Guarda el libro de trabajo
            workbook.Save("FillFormatPatternDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [FillPattern](../../fillpattern/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)



---
title: "FillFormat.GradientStyle"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad FillFormat. Devuelve el estilo de degradado para el relleno especificado"
type: docs
url: /es/net/aspose.cells.drawing/fillformat/gradientstyle/
---
## FillFormat.GradientStyle property

Devuelve el estilo de degradado para el relleno especificado.

```csharp
public GradientStyleType GradientStyle { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class FillFormatPropertyGradientStyleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Crea un gráfico y obtén su área del gráfico
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 5, 15, 15);
            Chart chart = sheet.Charts[chartIndex];
            ChartArea chartArea = chart.ChartArea;
            
            // Establece el estilo de relleno degradado
            chartArea.Area.FillFormat.SetPresetColorGradient(GradientPresetType.CalmWater, GradientStyleType.Vertical, 2);
            
            // Demuestra el uso de la propiedad GradientStyle
            Console.WriteLine("Gradient Style: " + chartArea.Area.FillFormat.GradientStyle);
            
            // Guarda el libro de trabajo
            workbook.Save("FillFormatPropertyGradientStyleDemo_out.xlsx");
        }
    }
}
```

### Ver también

* enum [GradientStyleType](../../gradientstyletype/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)



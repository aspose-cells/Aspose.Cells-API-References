---
title: "PatternFill.Pattern"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PatternFill. Obtiene o establece el tipo de patrón de relleno"
type: docs
url: /es/net/aspose.cells.drawing/patternfill/pattern/
---
## PatternFill.Pattern property

Obtiene o establece el tipo de patrón de relleno

```csharp
public FillPattern Pattern { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class PatternFillPropertyPatternDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Añade un gráfico
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Agregar datos de ejemplo para el gráfico
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["A2"].PutValue("Product A");
            worksheet.Cells["A3"].PutValue("Product B");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);
            
            // Establecer rango de datos del gráfico
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";
            
            // Establece el patrón de relleno para la primera serie
            chart.NSeries[0].Area.FillFormat.FillType = FillType.Pattern;
            chart.NSeries[0].Area.FillFormat.PatternFill.Pattern = FillPattern.WideDownwardDiagonal;
            
            // Guarda el libro de trabajo
            workbook.Save("PatternFillDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [FillPattern](../../fillpattern/)
* class [PatternFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)



---
title: "Line.BeginType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Line. Especifica una punta de flecha para el inicio de una línea"
type: docs
url: /es/net/aspose.cells.drawing/line/begintype/
---
## Line.BeginType property

Especifica una punta de flecha para el inicio de una línea.

```csharp
public MsoArrowheadStyle BeginType { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class LinePropertyBeginTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);

            // Agregar un gráfico de líneas
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Establecer origen de datos del Chart
            chart.NSeries.Add("A1:A3", true);

            // Obtener la primera serie y configurar sus propiedades de línea
            Series series = chart.NSeries[0];
            series.Border.BeginType = MsoArrowheadStyle.Arrow;
            series.Border.EndType = MsoArrowheadStyle.ArrowDiamond;
            series.Border.Color = Color.Red;
            series.Border.Weight = WeightType.MediumLine;

            // Guarda el libro de trabajo
            workbook.Save("LinePropertyBeginTypeDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [MsoArrowheadStyle](../../msoarrowheadstyle/)
* class [Line](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)



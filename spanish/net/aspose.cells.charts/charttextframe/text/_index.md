---
title: "ChartTextFrame.Text"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ChartTextFrame. Obtiene o establece el texto del título de un marco"
type: docs
url: /es/net/aspose.cells.charts/charttextframe/text/
---
## ChartTextFrame.Text property

Obtiene o establece el texto del título de un marco.

```csharp
public virtual string Text { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartTextFramePropertyTextDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            Cells cells = sheet.Cells;
            cells["A1"].PutValue("Category");
            cells["A2"].PutValue("A");
            cells["A3"].PutValue("B");
            cells["A4"].PutValue("C");
            cells["B1"].PutValue("Value");
            cells["B2"].PutValue(10);
            cells["B3"].PutValue(20);
            cells["B4"].PutValue(30);

            // Agregar gráfico
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = sheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B4", true);

            // Establecer texto del título del gráfico
            chart.Title.Text = "Sample Chart Title";

            // Acceder y modificar el texto de la leyenda
            Legend legend = chart.Legend;
            legend.Text = "Custom Legend Text";

            // Guarda el libro de trabajo
            workbook.Save("ChartTextDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ChartTextFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)



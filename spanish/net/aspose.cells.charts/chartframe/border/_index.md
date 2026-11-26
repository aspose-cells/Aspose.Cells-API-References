---
title: "ChartFrame.Border"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ChartFrame. Obtiene el borde"
type: docs
url: /es/net/aspose.cells.charts/chartframe/border/
---
## ChartFrame.Border property

Obtiene el [`border`](../../../aspose.cells.drawing/line/).

```csharp
public virtual Line Border { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ChartFramePropertyBorderDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
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

            // Agregar un gráfico de columnas
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.SetChartDataRange("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Acceder al título del gráfico
            chart.Title.Text = "Chart Title with Custom Border";
            ChartFrame title = chart.Title;

            // Configurar propiedades del borde
            Line border = title.Border;
            border.Color = System.Drawing.Color.Red;
            border.Style = LineType.Solid;
            border.Weight = WeightType.MediumLine;
            border.Transparency = 0.3;
            border.DashType = MsoLineDashStyle.Solid;

            // Guardar el resultado
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [Line](../../../aspose.cells.drawing/line/)
* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)



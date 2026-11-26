---
title: "ChartFrame.IsInnerMode"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ChartFrame. Indica si el tamaño del área de trazado incluye las marcas de graduación y las etiquetas de los ejes. False especifica que el tamaño determinará el tamaño del área de trazado, las marcas de graduación y las etiquetas de los ejes"
type: docs
url: /es/net/aspose.cells.charts/chartframe/isinnermode/
---
## ChartFrame.IsInnerMode property

Indica si el tamaño del área de trazado incluye las marcas de graduación y las etiquetas de los ejes. False especifica que el tamaño determinará el tamaño del área de trazado, las marcas de graduación y las etiquetas de los ejes.

```csharp
public bool IsInnerMode { get; set; }
```

### Observaciones

Solo para archivo Xlsx.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class ChartFramePropertyIsInnerModeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Agregar gráfico
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Acceder al marco del gráfico y demostrar IsInnerMode
            Aspose.Cells.Charts.ChartFrame chartFrame = chart.ChartArea;
            chartFrame.IsInnerMode = true; // Set to use inner mode
            
            // Establecer algunas propiedades básicas para mostrar el efecto
            chartFrame.Border.Color = Color.Blue;
            chartFrame.Border.Style = Aspose.Cells.Drawing.LineType.Solid;
            chartFrame.Area.ForegroundColor = Color.LightYellow;

            workbook.Save("ChartFrameIsInnerModeDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)



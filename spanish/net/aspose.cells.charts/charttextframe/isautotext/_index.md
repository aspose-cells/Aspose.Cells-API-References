---
title: "ChartTextFrame.IsAutoText"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ChartTextFrame. Indica que el texto se genera automáticamente"
type: docs
url: /es/net/aspose.cells.charts/charttextframe/isautotext/
---
## ChartTextFrame.IsAutoText property

Indica que el texto se genera automáticamente.

```csharp
public virtual bool IsAutoText { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartTextFramePropertyIsAutoTextDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo para el gráfico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Añade un gráfico
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];

            // Establecer datos del gráfico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Configurar el título del gráfico
            Aspose.Cells.Charts.ChartTextFrame title = chart.Title;
            title.Text = "Custom Chart Title";
            
            // Demostrar la propiedad IsAutoText
            title.IsAutoText = false; // Disable auto-generated text
            
            // Guarda el libro de trabajo
            workbook.Save("ChartTextFrame_IsAutoText_Demo.xlsx");
        }
    }
}
```

### Ver también

* class [ChartTextFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)



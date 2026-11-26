---
title: "ChartTextFrame.IsTextWrapped"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ChartTextFrame. Obtiene o establece un valor que indica si el texto está ajustado"
type: docs
url: /es/net/aspose.cells.charts/charttextframe/istextwrapped/
---
## ChartTextFrame.IsTextWrapped property

Obtiene o establece un valor que indica si el texto está ajustado.

```csharp
public virtual bool IsTextWrapped { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ChartTextFramePropertyIsTextWrappedDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("Q1");
            sheet.Cells["A3"].PutValue("Q2");
            sheet.Cells["B1"].PutValue("Sales");
            sheet.Cells["B2"].PutValue(12000);
            sheet.Cells["B3"].PutValue(15000);

            // Agregar gráfico
            int chartIndex = sheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 5, 20, 10);
            Chart chart = sheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            // Establecer el título del gráfico con ajuste de texto
            chart.Title.Text = "Quarterly Sales Report (2023) - This is a long title that will wrap when IsTextWrapped is true";
            chart.Title.IsTextWrapped = true;
            
            // Guardar el libro de trabajo
            workbook.Save("ChartTextWrappingDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ChartTextFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)



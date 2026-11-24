---
title: "ChartTextFrame.IsTextWrapped"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ChartTextFrame-Eigenschaft. Gibt einen Wert zurück oder legt ihn fest, der angibt, ob der Text umgebrochen ist"
type: docs
url: /de/net/aspose.cells.charts/charttextframe/istextwrapped/
---
## ChartTextFrame.IsTextWrapped property

Liest oder legt einen Wert fest, der angibt, ob der Text umgebrochen wird.

```csharp
public virtual bool IsTextWrapped { get; set; }
```

### Beispiele

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

            // Fügen Sie Beispieldaten hinzu
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("Q1");
            sheet.Cells["A3"].PutValue("Q2");
            sheet.Cells["B1"].PutValue("Sales");
            sheet.Cells["B2"].PutValue(12000);
            sheet.Cells["B3"].PutValue(15000);

            // Diagramm hinzufügen
            int chartIndex = sheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 5, 20, 10);
            Chart chart = sheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            // Diagrammtitel mit Textumbruch festlegen
            chart.Title.Text = "Quarterly Sales Report (2023) - This is a long title that will wrap when IsTextWrapped is true";
            chart.Title.IsTextWrapped = true;
            
            // Arbeitsmappe speichern.
            workbook.Save("ChartTextWrappingDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ChartTextFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)



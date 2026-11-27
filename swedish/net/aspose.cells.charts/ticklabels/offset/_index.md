---
title: "TickLabels.Offset"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TickLabels‑egenskap. Hämtar och anger avståndet för etiketter från kategori‑axeln. Detta gäller endast för kategori‑x‑axeln"
type: docs
url: /sv/net/aspose.cells.charts/ticklabels/offset/
---
## TickLabels.Offset property

Hämtar och anger avståndet för etiketter från kategoriaxeln. Detta gäller endast kategori‑(x‑)axeln.

```csharp
public int Offset { get; set; }
```

### Anmärkningar

Standardavståndet är 100 procent, vilket representerar standardavståndet mellan axel­etiketterna och axellinjen. Värdet kan vara ett heltal i procent från 0 till 1000, relativt axel­etikettens teckenstorlek.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class TickLabelsPropertyOffsetDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["A4"].PutValue("C");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["B3"].PutValue(20);
            sheet.Cells["B4"].PutValue(30);

            // Lägg till ett diagram
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = sheet.Charts[chartIndex];
            
            // Ställ in diagramdatakälla
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Åtkomst till värdeaxeln
            Axis valueAxis = chart.ValueAxis;
            
            // Ange TickLabels‑offset
            valueAxis.TickLabels.Offset = 50; // 50% offset from default position

            // Spara arbetsboken
            workbook.Save("TickLabelsOffsetDemo.xlsx");
        }
    }
}
```

### Se även

* class [TickLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)



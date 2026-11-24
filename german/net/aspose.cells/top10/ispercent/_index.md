---
title: "Top10.IsPercent"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Top10-Eigenschaft. Liest oder setzt, ob eine Top/Bottom-n-Regel eine Top/Bottom-n-Prozent-Regel ist. Standardwert ist false"
type: docs
url: /de/net/aspose.cells/top10/ispercent/
---
## Top10.IsPercent property

Abrufen oder Festlegen, ob eine „top/bottom n“-Regel eine „top/bottom n percent“-Regel ist. Standardwert ist false.

```csharp
public bool IsPercent { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class Top10PropertyIsPercentDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells[i, 0].PutValue(i + 1);
            }

            // Füge eine Top10-Regel für bedingte Formatierung hinzu
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];
            fcc.AddCondition(FormatConditionType.Top10, OperatorType.None, null, null);

            // Lese die Top10-Formatbedingung
            FormatCondition fc = fcc[0];
            
            // Setze Top10-Eigenschaften
            fc.Top10.IsPercent = true;  // Demonstrate IsPercent property
            fc.Top10.IsBottom = false;
            fc.Top10.Rank = 3;

            // Wenden Sie den Formatierungsstil an
            Style style = workbook.CreateStyle();
            style.Font.Color = System.Drawing.Color.Red;
            fc.Style = style;

            // Speichere die Arbeitsmappe
            workbook.Save("Top10IsPercentDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Top10](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



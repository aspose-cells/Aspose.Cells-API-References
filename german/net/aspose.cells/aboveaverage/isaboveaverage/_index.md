---
title: "AboveAverage.IsAboveAverage"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "AboveAverage-Eigenschaft. Gibt das Flag an oder legt es fest, ob die Regel eine überdurchschnittliche Regel ist. true bedeutet überdurchschnittlich. Der Standardwert ist true"
type: docs
url: /de/net/aspose.cells/aboveaverage/isaboveaverage/
---
## AboveAverage.IsAboveAverage property

Lese oder setze das Flag, das angibt, ob die Regel eine „above average“-Regel ist. 'true' bedeutet 'above average'. Standardwert ist true.

```csharp
public bool IsAboveAverage { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class AboveAveragePropertyIsAboveAverageDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Workbook
            Workbook workbook = new Workbook();
            
            // Hole das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge Beispieldaten hinzu, um die bedingte Formatierung zu demonstrieren
            for (int i = 0; i <= 10; i++)
            {
                worksheet.Cells[i, 0].PutValue(i * 10);
            }

            // Eine bedingte Formatierung hinzufügen
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];

            // Den Bereich der bedingten Formatierung festlegen
            CellArea ca = new CellArea
            {
                StartRow = 0,
                EndRow = 10,
                StartColumn = 0,
                EndColumn = 0
            };
            fcs.AddArea(ca);

            // Eine AboveAverage-Bedingung hinzufügen
            int conditionIndex = fcs.AddCondition(FormatConditionType.AboveAverage);
            FormatCondition fc = fcs[conditionIndex];
            fc.Style.BackgroundColor = Color.Yellow;

            // Die AboveAverage-Eigenschaften konfigurieren
            fc.AboveAverage.IsAboveAverage = true;  // Highlight values above average
            fc.AboveAverage.IsEqualAverage = false; // Exclude values equal to average

            // Speichere die Excel-Datei
            workbook.Save("AboveAverageConditionDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [AboveAverage](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



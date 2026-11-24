---
title: "Worksheet.ConditionalFormattings"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Worksheet-Eigenschaft. Gibt die ConditionalFormattings im Arbeitsblatt zurück"
type: docs
url: /de/net/aspose.cells/worksheet/conditionalformattings/
---
## Worksheet.ConditionalFormattings property

Liest die ConditionalFormattings im Arbeitsblatt.

```csharp
public ConditionalFormattingCollection ConditionalFormattings { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyConditionalFormattingsDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            sheet.Cells["A1"].PutValue(10);
            sheet.Cells["A2"].PutValue(20);
            sheet.Cells["A3"].PutValue(30);

            // Bedingte Formatierung erstellen
            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = sheet.ConditionalFormattings[index];
            
            // Bereich festlegen
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 2;
            area.EndColumn = 0;
            fcc.AddArea(area);

            // Bedingung hinzufügen
            int conditionIndex = fcc.AddCondition(FormatConditionType.CellValue, OperatorType.GreaterThan, "15", null);
            FormatCondition fc = fcc[conditionIndex];
            fc.Style.BackgroundColor = System.Drawing.Color.Red;

            // Speichere die Arbeitsmappe
            workbook.Save("ConditionalFormattingDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ConditionalFormattingCollection](../../conditionalformattingcollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



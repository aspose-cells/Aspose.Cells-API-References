---
title: "FormatCondition.Priority"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "FormatCondition-Eigenschaft. Die Priorität dieser bedingten Formatierungsregel. Dieser Wert wird verwendet, um zu bestimmen, welches Format ausgewertet und gerendert werden soll. Niedrigere numerische Werte haben höhere Priorität als höhere numerische Werte, wobei 1 die höchste Priorität darstellt."
type: docs
url: /de/net/aspose.cells/formatcondition/priority/
---
## FormatCondition.Priority property

Die Priorität dieser Regel für bedingte Formatierung. Dieser Wert wird verwendet, um zu bestimmen, welches Format ausgewertet und gerendert werden soll. Niedrigere numerische Werte haben höhere Priorität als höhere numerische Werte, wobei '1' die höchste Priorität hat.

```csharp
public int Priority { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormatConditionPropertyPriorityDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            for (int i = 0; i < 10; i++)
            {
                sheet.Cells[i, 0].PutValue(i + 1);
            }

            // Bedingte Formatierung hinzufügen
            int formatIndex = sheet.ConditionalFormattings.Add();
            FormatConditionCollection formatConditions = sheet.ConditionalFormattings[formatIndex];
            
            // Bedingungen hinzufügen
            int conditionIndex1 = formatConditions.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "2", "5");
            int conditionIndex2 = formatConditions.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "6", "9");

            // Prioritäten festlegen
            formatConditions[conditionIndex1].Priority = 2;
            formatConditions[conditionIndex2].Priority = 1;

            // Demonstrieren Sie die Verwendung der Priority-Eigenschaft
            Console.WriteLine("Condition 1 Priority: " + formatConditions[conditionIndex1].Priority);
            Console.WriteLine("Condition 2 Priority: " + formatConditions[conditionIndex2].Priority);

            // Speichere die Arbeitsmappe
            workbook.Save("ConditionalFormattingPriorityDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



---
title: "FormatCondition.Text"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "FormatCondition-Eigenschaft. Der Textwert in einer Text‑enthält‑bedingte‑Formatierungs‑Regel. Gültig nur für die Typen containsText, notContainsText, beginsWith und endsWith. Der Standardwert ist null."
type: docs
url: /de/net/aspose.cells/formatcondition/text/
---
## FormatCondition.Text property

Der Textwert in einer "text contains"-Regel für bedingte Formatierung. Gültig nur für Typ = containsText, notContainsText, beginsWith und endsWith. Der Standardwert ist null.

```csharp
public string Text { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class FormatConditionPropertyTextDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Bedingte Formatierung hinzufügen
            ConditionalFormattingCollection conditionalFormattings = sheet.ConditionalFormattings;
            int collectionIndex = conditionalFormattings.Add();
            FormatConditionCollection formatConditions = conditionalFormattings[collectionIndex];

            // Fügen Sie eine Textbedingung hinzu
            int conditionIndex = formatConditions.AddCondition(FormatConditionType.ContainsText);
            FormatCondition formatCondition = formatConditions[conditionIndex];
            
            // Setzen Sie die Texteigenschaft (demonstriert russischen Text)
            formatCondition.Text = "вс";

            // Wenden Sie den Formatierungsstil an
            Style style = formatCondition.Style;
            style.BackgroundColor = Color.Red;
            formatCondition.Style = style;

            // Auf Zelle A1 anwenden
            formatConditions.AddArea(CellArea.CreateCellArea("A1", "A1"));

            // Speichern und überprüfen
            string outputPath = "FormatConditionPropertyTextDemo_Output.xlsx";
            workbook.Save(outputPath);

            Console.WriteLine("FormatCondition Text property demo completed successfully.");
        }
    }
}
```

### Siehe auch

* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



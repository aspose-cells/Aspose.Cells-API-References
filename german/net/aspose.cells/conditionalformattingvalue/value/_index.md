---
title: "ConditionalFormattingValue.Value"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ConditionalFormattingValue‑Eigenschaft. Gibt den Wert dieses bedingten Formatierungswert‑Objekts zurück oder legt ihn fest. Sie sollte zusammen mit Type verwendet werden."
type: docs
url: /de/net/aspose.cells/conditionalformattingvalue/value/
---
## ConditionalFormattingValue.Value property

Abrufen oder Festlegen des Werts dieses bedingten Formatierungswertobjekts. Es sollte zusammen mit Type verwendet werden.

```csharp
public object Value { get; set; }
```

### Hinweise

Wenn der Wert ein String ist und mit \"=\" beginnt, wird er als Formel verarbeitet, andernfalls verarbeiten wir ihn als einfachen Wert.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ConditionalFormattingValuePropertyValueDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(40);

            // Bedingte Formatierung hinzufügen
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];
            
            // Bedingte Formatierung für Symbolsatz erstellen
            int conditionIndex = fcc.AddCondition(FormatConditionType.IconSet);
            FormatCondition condition = fcc[conditionIndex];
            condition.IconSet.Type = IconSetType.Arrows3;

            // Hole die Objekte für bedingte Formatierungswerte
            ConditionalFormattingValueCollection cfvos = condition.IconSet.Cfvos;

            // Setze Werte für die Symbole
            cfvos[0].Type = FormatConditionValueType.Min;
            cfvos[0].Value = 0;
            
            cfvos[1].Type = FormatConditionValueType.Percent;
            cfvos[1].Value = 33;
            
            cfvos[2].Type = FormatConditionValueType.Percent;
            cfvos[2].Value = 67;

            // Demonstriere die Verwendung der Value‑Eigenschaft
            Console.WriteLine("First icon value: " + cfvos[0].Value);
            Console.WriteLine("Second icon value: " + cfvos[1].Value);
            Console.WriteLine("Third icon value: " + cfvos[2].Value);

            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [ConditionalFormattingValue](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



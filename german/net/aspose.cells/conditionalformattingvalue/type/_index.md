---
title: "ConditionalFormattingValue.Type"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ConditionalFormattingValue-Eigenschaft. Gibt den Typ dieses bedingten Formatierungswertobjekts zurück oder legt ihn fest. Das Festlegen des Typs auf FormatConditionValueType.Min oder FormatConditionValueType.Max setzt Value automatisch auf null."
type: docs
url: /de/net/aspose.cells/conditionalformattingvalue/type/
---
## ConditionalFormattingValue.Type property

Abrufen oder Festlegen des Typs dieses bedingten Formatierungswertobjekts. Das Setzen des Typs auf FormatConditionValueType.Min oder FormatConditionValueType.Max setzt "Value" automatisch auf null.

```csharp
public FormatConditionValueType Type { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ConditionalFormattingValuePropertyTypeDemo
    {
        public static void Run()
        {
            try
            {
                // Erstelle ein neues Arbeitsbuch
                Workbook workbook = new Workbook();
                Worksheet ws = workbook.Worksheets[0];

                // Fügen Sie einige Beispieldaten hinzu (erforderlich, damit bedingte Formatierung existiert).
                ws.Cells["A1"].PutValue(10);
                ws.Cells["A2"].PutValue(20);
                ws.Cells["A3"].PutValue(30);

                // Erstellen Sie eine Sammlung für bedingte Formatierung und fügen Sie eine IconSet-Bedingung hinzu.
                int cfIndex = ws.ConditionalFormattings.Add();
                FormatConditionCollection fcc = ws.ConditionalFormattings[cfIndex];

                int condIdx = fcc.AddCondition(FormatConditionType.IconSet);
                FormatCondition condition = fcc[condIdx];
                condition.IconSet.Type = IconSetType.Arrows3; // any valid icon set type

                // Holen Sie eine ConditionalFormattingValue-Instanz aus der IconSet-Sammlung.
                ConditionalFormattingValue cfv = condition.IconSet.Cfvos[0];

                // Setzen Sie den Typ auf Percent und weisen Sie einen entsprechenden Wert zu.
                cfv.Type = FormatConditionValueType.Percent;
                cfv.Value = 25; // 25%

                // Lesen und zeigen Sie den Typ und Value an.
                Console.WriteLine("After setting Type to Percent:");
                Console.WriteLine("  Type : " + cfv.Type);
                Console.WriteLine("  Value: " + cfv.Value);

                // Ändern Sie den Typ zu Min – laut Dokumentation wird dadurch Value auf null gesetzt.
                cfv.Type = FormatConditionValueType.Min;

                // Lesen und zeigen Sie den Typ und Value erneut an.
                Console.WriteLine("\nAfter setting Type to Min:");
                Console.WriteLine("  Type : " + cfv.Type);
                Console.WriteLine("  Value: " + (cfv.Value == null ? "null" : cfv.Value.ToString()));

                // Speichern Sie die Arbeitsmappe (die bedingte Formatierung ist Teil des Blatts).
                workbook.Save("ConditionalFormattingValueTypeDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* enum [FormatConditionValueType](../../formatconditionvaluetype/)
* class [ConditionalFormattingValue](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



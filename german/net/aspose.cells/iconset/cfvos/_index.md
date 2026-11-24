---
title: "IconSet.Cfvos"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "IconSet-Eigenschaft. Gibt die CFValueObjects-Instanz zurück"
type: docs
url: /de/net/aspose.cells/iconset/cfvos/
---
## IconSet.Cfvos property

Abrufen der CFValueObjects-Instanz.

```csharp
public ConditionalFormattingValueCollection Cfvos { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class IconSetPropertyCfvosDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells[i, 0].PutValue(i * 10);
            }

            try
            {
                // Bedingte Formatierung hinzufügen
                int cfIndex = worksheet.ConditionalFormattings.Add();
                FormatConditionCollection fcs = worksheet.ConditionalFormattings[cfIndex];

                // Bereich für bedingte Formatierung festlegen
                CellArea area = new CellArea();
                area.StartRow = 0;
                area.StartColumn = 0;
                area.EndRow = 9;
                area.EndColumn = 0;
                fcs.AddArea(area);

                // Symbolsatz-Bedingung hinzufügen
                int conditionIndex = fcs.AddCondition(FormatConditionType.IconSet);
                FormatCondition condition = fcs[conditionIndex];

                // Symbolsatztyp festlegen
                condition.IconSet.Type = IconSetType.TrafficLights31;

                // Zugriff auf die Cfvos-Eigenschaft (schreibgeschützt)
                ConditionalFormattingValueCollection cfvos = condition.IconSet.Cfvos;

                // Informationen über die Cfvos-Sammlung anzeigen
                Console.WriteLine("Number of CFValueObjects in the collection: " + cfvos.Count);

                // Durch die Sammlung iterieren und jeden Wert anzeigen
                for (int i = 0; i < cfvos.Count; i++)
                {
                    ConditionalFormattingValue cfValue = cfvos[i];
                    Console.WriteLine($"CFValue {i + 1}: Type = {cfValue.Type}, Value = {cfValue.Value}");
                }

                // Speichere die Arbeitsmappe
                workbook.Save("IconSetCfvosDemo.xlsx");
                Console.WriteLine("Workbook saved successfully with icon set conditional formatting.");
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

* class [ConditionalFormattingValueCollection](../../conditionalformattingvaluecollection/)
* class [IconSet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



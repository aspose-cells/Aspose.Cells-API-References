---
title: "IconSet.Cfvos"
second_title: "Aspose.Cells för .NET API‑referens"
description: "IconSet-egenskap. Hämta CFValueObjects-instansen"
type: docs
url: /sv/net/aspose.cells/iconset/cfvos/
---
## IconSet.Cfvos property

Hämta CFValueObjects-instansen.

```csharp
public ConditionalFormattingValueCollection Cfvos { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class IconSetPropertyCfvosDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells[i, 0].PutValue(i * 10);
            }

            try
            {
                // Lägg till villkorsstyrd formatering
                int cfIndex = worksheet.ConditionalFormattings.Add();
                FormatConditionCollection fcs = worksheet.ConditionalFormattings[cfIndex];

                // Ange intervall för villkorsformatering
                CellArea area = new CellArea();
                area.StartRow = 0;
                area.StartColumn = 0;
                area.EndRow = 9;
                area.EndColumn = 0;
                fcs.AddArea(area);

                // Lägg till ikonsetvillkor
                int conditionIndex = fcs.AddCondition(FormatConditionType.IconSet);
                FormatCondition condition = fcs[conditionIndex];

                // Ange ikonsettyp
                condition.IconSet.Type = IconSetType.TrafficLights31;

                // Åtkomst till Cfvos-egenskapen (skrivskyddad)
                ConditionalFormattingValueCollection cfvos = condition.IconSet.Cfvos;

                // Visa information om Cfvos-samlingen
                Console.WriteLine("Number of CFValueObjects in the collection: " + cfvos.Count);

                // Iterera genom samlingen och visa varje värde
                for (int i = 0; i < cfvos.Count; i++)
                {
                    ConditionalFormattingValue cfValue = cfvos[i];
                    Console.WriteLine($"CFValue {i + 1}: Type = {cfValue.Type}, Value = {cfValue.Value}");
                }

                // Spara arbetsboken
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

### Se även

* class [ConditionalFormattingValueCollection](../../conditionalformattingvaluecollection/)
* class [IconSet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



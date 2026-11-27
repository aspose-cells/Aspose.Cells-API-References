---
title: "ConditionalFormattingValueCollection.Item"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ConditionalFormattingValueCollection-egenskap. Hämta CFValueObject-elementet på det angivna indexet"
type: docs
url: /sv/net/aspose.cells/conditionalformattingvaluecollection/item/
---
## ConditionalFormattingValueCollection indexer

Hämta CFValueObject-elementet på det angivna indexet.

```csharp
public ConditionalFormattingValue this[int index] { get; }
```

| Parameter | Beskrivning |
| --- | --- |
| index | Det nollbaserade indexet för elementet. |

### Returvärde

Elementet på det angivna indexet.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ConditionalFormattingValueCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Lägg till exempeldata
                worksheet.Cells["A1"].PutValue(10);
                worksheet.Cells["A2"].PutValue(120);
                worksheet.Cells["A3"].PutValue(260);

                // Lägg till villkorsstyrd formatering
                int cfIndex = worksheet.ConditionalFormattings.Add();
                FormatConditionCollection fcs = worksheet.ConditionalFormattings[cfIndex];

                // Ange intervallet för villkorlig formatering
                CellArea ca = new CellArea
                {
                    StartRow = 0,
                    EndRow = 2,
                    StartColumn = 0,
                    EndColumn = 0
                };
                fcs.AddArea(ca);

                // Lägg till ett ikonsetvillkor
                int conditionIndex = fcs.AddCondition(FormatConditionType.IconSet);
                FormatCondition condition = fcs[conditionIndex];
                IconSet iconSet = condition.IconSet;
                iconSet.Type = IconSetType.Arrows3;

                // Hämta ConditionalFormattingValueCollection
                ConditionalFormattingValueCollection cfvos = iconSet.Cfvos;

                // Lägg till ett värde i samlingen
                int valueIndex = cfvos.Add(FormatConditionValueType.Number, "50");

                // Demonstrera åtkomst till Item-egenskapen (indexerare)
                ConditionalFormattingValue cfv = cfvos[valueIndex];

                // Visa värdet från Item-egenskapen
                Console.WriteLine($"Conditional Formatting Value at index {valueIndex}:");
                Console.WriteLine($"  Type: {cfv.Type}");
                Console.WriteLine($"  Value: {cfv.Value}");
                Console.WriteLine($"  IsGTE: {cfv.IsGTE}");

                // Spara arbetsboken
                workbook.Save("ConditionalFormattingValueCollectionItemDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
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

* class [ConditionalFormattingValue](../../conditionalformattingvalue/)
* class [ConditionalFormattingValueCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



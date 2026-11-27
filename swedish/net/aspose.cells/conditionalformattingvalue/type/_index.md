---
title: "ConditionalFormattingValue.Type"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ConditionalFormattingValue-egenskap. Hämta eller ange typen för detta villkorliga formateringsvärdeobjekt. Att ange typen till FormatConditionValueType.Min eller FormatConditionValueType.Max kommer automatiskt att sätta Value till null"
type: docs
url: /sv/net/aspose.cells/conditionalformattingvalue/type/
---
## ConditionalFormattingValue.Type property

Hämta eller ange typen för detta villkorsformateringsvärdeobjekt. Att ange typen till FormatConditionValueType.Min eller FormatConditionValueType.Max kommer automatiskt att sätta "Value" till null.

```csharp
public FormatConditionValueType Type { get; set; }
```

### Exempel

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
                // Skapa en ny arbetsbok
                Workbook workbook = new Workbook();
                Worksheet ws = workbook.Worksheets[0];

                // Lägg till några exempeldata (krävs för att villkorlig formatering ska finnas)
                ws.Cells["A1"].PutValue(10);
                ws.Cells["A2"].PutValue(20);
                ws.Cells["A3"].PutValue(30);

                // Skapa en samling för villkorlig formatering och lägg till ett IconSet-villkor
                int cfIndex = ws.ConditionalFormattings.Add();
                FormatConditionCollection fcc = ws.ConditionalFormattings[cfIndex];

                int condIdx = fcc.AddCondition(FormatConditionType.IconSet);
                FormatCondition condition = fcc[condIdx];
                condition.IconSet.Type = IconSetType.Arrows3; // any valid icon set type

                // Hämta en ConditionalFormattingValue-instans från IconSet-samlingen
                ConditionalFormattingValue cfv = condition.IconSet.Cfvos[0];

                // Ställ in Type till Percent och tilldela ett motsvarande värde
                cfv.Type = FormatConditionValueType.Percent;
                cfv.Value = 25; // 25%

                // Läs och visa Type och Value
                Console.WriteLine("After setting Type to Percent:");
                Console.WriteLine("  Type : " + cfv.Type);
                Console.WriteLine("  Value: " + cfv.Value);

                // Ändra Type till Min – enligt dokumentationen kommer detta att nollställa Value
                cfv.Type = FormatConditionValueType.Min;

                // Läs och visa Type och Value igen
                Console.WriteLine("\nAfter setting Type to Min:");
                Console.WriteLine("  Type : " + cfv.Type);
                Console.WriteLine("  Value: " + (cfv.Value == null ? "null" : cfv.Value.ToString()));

                // Spara arbetsboken (villkorlig formatering är en del av bladet)
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

### Se även

* enum [FormatConditionValueType](../../formatconditionvaluetype/)
* class [ConditionalFormattingValue](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



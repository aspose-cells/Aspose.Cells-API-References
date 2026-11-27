---
title: "ConditionalFormattingValue.Value"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ConditionalFormattingValue‑egenskap. Hämta eller ange värdet för detta villkorliga formateringsvärdesobjekt. Den bör användas tillsammans med Type"
type: docs
url: /sv/net/aspose.cells/conditionalformattingvalue/value/
---
## ConditionalFormattingValue.Value property

Hämta eller ange värdet för detta villkorsformateringsvärdeobjekt. Det bör användas tillsammans med Type.

```csharp
public object Value { get; set; }
```

### Anmärkningar

Om värdet är en sträng och börjar med "=", behandlas det som en formel, annars behandlar vi det som ett enkelt värde.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ConditionalFormattingValuePropertyValueDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(40);

            // Lägg till villkorsstyrd formatering
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];
            
            // Skapa villkorsformatering för ikonset
            int conditionIndex = fcc.AddCondition(FormatConditionType.IconSet);
            FormatCondition condition = fcc[conditionIndex];
            condition.IconSet.Type = IconSetType.Arrows3;

            // Hämta de villkorliga formateringsvärdeobjekten
            ConditionalFormattingValueCollection cfvos = condition.IconSet.Cfvos;

            // Ange värden för ikonerna
            cfvos[0].Type = FormatConditionValueType.Min;
            cfvos[0].Value = 0;
            
            cfvos[1].Type = FormatConditionValueType.Percent;
            cfvos[1].Value = 33;
            
            cfvos[2].Type = FormatConditionValueType.Percent;
            cfvos[2].Value = 67;

            // Demonstrera användning av Value‑egenskapen
            Console.WriteLine("First icon value: " + cfvos[0].Value);
            Console.WriteLine("Second icon value: " + cfvos[1].Value);
            Console.WriteLine("Third icon value: " + cfvos[2].Value);

            // Spara arbetsboken
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [ConditionalFormattingValue](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



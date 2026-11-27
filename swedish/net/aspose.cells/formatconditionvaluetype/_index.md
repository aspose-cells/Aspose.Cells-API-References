---
title: "Enum FormatConditionValueType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.FormatConditionValueType enum. Villkorsvärdestyp"
type: docs
url: /sv/net/aspose.cells/formatconditionvaluetype/
---
## FormatConditionValueType enumeration

Villkorligt värdetyp.

```csharp
public enum FormatConditionValueType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Formula | `0` | Det minsta/mellan-/största värdet för gradienten bestäms av en formel. |
| Max | `1` | Indikerar att det största värdet i intervallet ska användas som det största värdet för gradienten. |
| Min | `2` | Indikerar att det minsta värdet i intervallet ska användas som det minsta värdet för gradienten. |
| Number | `3` | Indikerar att det minsta/mellan-/största värdet för gradienten specificeras av ett konstant numeriskt värde. |
| Percent | `4` | Värdet indikerar att en procentsats mellan det minsta och största värdet i intervallet ska användas som det minsta/mellan-/största värdet för gradienten. |
| Percentile | `5` | Värdet indikerar att en percentilrankning i intervallet ska användas som det minsta/mellan-/största värdet för gradienten. |
| AutomaticMax | `6` | Indikerar att det automatiska största värdet i intervallet ska användas som det automatiska största värdet för gradienten. |
| AutomaticMin | `7` | Indikerar att det automatiska minsta värdet i intervallet ska användas som det automatiska minsta värdet för gradienten. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassFormatConditionValueTypeDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till formatvillkor
            int formatConditionsIndex = sheet.ConditionalFormattings.Add();
            FormatConditionCollection formatConditions = sheet.ConditionalFormattings[formatConditionsIndex];
            int conditionIndex = formatConditions.AddCondition(FormatConditionType.IconSet);
            FormatCondition condition = formatConditions[conditionIndex];

            // Ställ in egenskaper för ikonsats
            condition.IconSet.Type = IconSetType.Boxes5;
            condition.IconSet.ShowValue = false;
            condition.IconSet.Reverse = true;

            // Ställ in cellvärde och tillämpa formatering
            Cell cell = sheet.Cells["A1"];
            cell.PutValue("Boxes5 Icon Set Example");

            // Åtkomst till formatvillkorsvärdestyp
            FormatConditionValueType valueType = condition.IconSet.Cfvos[0].Type;
            Console.WriteLine("First CFVO Type: " + valueType);

            // Visa värden från ikonsatsvillkoren
            Console.WriteLine("\nIcon Set Threshold Values:");
            foreach (ConditionalFormattingValue cfvo in condition.IconSet.Cfvos)
            {
                Console.WriteLine($"Type: {cfvo.Type}, Value: {cfvo.Value}");
            }

            // Spara arbetsboken
            workbook.Save("FormatConditionValueTypeDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)



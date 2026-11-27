---
title: "FormatCondition.Priority"
second_title: "Aspose.Cells för .NET API‑referens"
description: "FormatCondition-egenskap. Prioriteten för denna villkorliga formateringsregel. Detta värde används för att avgöra vilken format som ska utvärderas och renderas. Lägre numeriska värden har högre prioritet än högre numeriska värden, där 1 är den högsta prioriteten."
type: docs
url: /sv/net/aspose.cells/formatcondition/priority/
---
## FormatCondition.Priority property

Prioriteten för denna villkorliga formateringsregel. Detta värde används för att avgöra vilket format som ska utvärderas och renderas. Lägre numeriska värden har högre prioritet än högre numeriska värden, där '1' är den högsta prioriteten.

```csharp
public int Priority { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormatConditionPropertyPriorityDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            for (int i = 0; i < 10; i++)
            {
                sheet.Cells[i, 0].PutValue(i + 1);
            }

            // Lägg till villkorsstyrd formatering
            int formatIndex = sheet.ConditionalFormattings.Add();
            FormatConditionCollection formatConditions = sheet.ConditionalFormattings[formatIndex];
            
            // Lägg till villkor
            int conditionIndex1 = formatConditions.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "2", "5");
            int conditionIndex2 = formatConditions.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "6", "9");

            // Ställ in prioriteringar
            formatConditions[conditionIndex1].Priority = 2;
            formatConditions[conditionIndex2].Priority = 1;

            // Demonstrera användning av Priority-egenskapen
            Console.WriteLine("Condition 1 Priority: " + formatConditions[conditionIndex1].Priority);
            Console.WriteLine("Condition 2 Priority: " + formatConditions[conditionIndex2].Priority);

            // Spara arbetsboken
            workbook.Save("ConditionalFormattingPriorityDemo.xlsx");
        }
    }
}
```

### Se även

* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



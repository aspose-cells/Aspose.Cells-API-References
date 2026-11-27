---
title: "FormatConditionCollection.RangeCount"
second_title: "Aspose.Cells för .NET API‑referens"
description: "FormatConditionCollection-egenskapen. Hämtar antalet villkorligt formaterade områden"
type: docs
url: /sv/net/aspose.cells/formatconditioncollection/rangecount/
---
## FormatConditionCollection.RangeCount property

Hämtar antalet villkorligt formaterade områden.

```csharp
public int RangeCount { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormatConditionCollectionPropertyRangeCountDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till lite exempeldata
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(40);

            // Lägg till villkorsstyrd formatering
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];
            
            // Lägg till områden med AddArea-metoden istället för AddRange
            fcc.AddArea(new CellArea { StartRow = 0, StartColumn = 0, EndRow = 3, EndColumn = 0 });
            fcc.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "10", "50");

            // Demonstrera RangeCount-egenskapen
            Console.WriteLine($"Number of ranges in FormatConditionCollection: {fcc.RangeCount}");
            
            // Validera RangeCount
            if (fcc.RangeCount < 1)
            {
                Console.WriteLine("Error: No ranges applied to conditional formatting");
            }
            else
            {
                Console.WriteLine("Conditional formatting ranges applied successfully");
            }
        }
    }
}
```

### Se även

* class [FormatConditionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



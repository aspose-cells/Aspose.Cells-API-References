---
title: "Worksheet.Index"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Worksheet-egenskap. Hämtar indexet för bladet i kalkylbladsamlingen"
type: docs
url: /sv/net/aspose.cells/worksheet/index/
---
## Worksheet.Index property

Hämtar indexet för bladet i kalkylblads samlingen.

```csharp
public int Index { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyIndexDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Lägg till tre kalkylblad
            workbook.Worksheets.Add("Sheet1");
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");

            // Åtkomst till kalkylblad via index och demonstrera Index-egenskapen
            Console.WriteLine("Worksheet Index Demonstration:");
            for (int i = 0; i < workbook.Worksheets.Count; i++)
            {
                Worksheet sheet = workbook.Worksheets[i];
                Console.WriteLine($"Worksheet Name: {sheet.Name}, Index: {sheet.Index}");
            }

            // Lägg till villkorsstyrd formatering för att demonstrera användning av index
            Worksheet firstSheet = workbook.Worksheets[0];
            int formatIndex = firstSheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = firstSheet.ConditionalFormattings[formatIndex];
            fcc.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "10", "100");
            
            // Visa information om index för villkorsstyrd formatering
            Console.WriteLine("\nConditional Formatting Indexes:");
            Console.WriteLine($"Worksheet Index: {firstSheet.Index}");
            Console.WriteLine($"Formatting Collection Index: {formatIndex}");
            Console.WriteLine($"First Condition Index: 0");
        }
    }
}
```

### Se även

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



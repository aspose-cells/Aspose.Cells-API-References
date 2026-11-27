---
title: "FormatCondition.Operator"
second_title: "Aspose.Cells för .NET API‑referens"
description: "FormatCondition-egenskap. Hämtar och anger typen av villkorsformateringsoperator"
type: docs
url: /sv/net/aspose.cells/formatcondition/operator/
---
## FormatCondition.Operator property

Hämtar och anger den villkorliga formatoperatorns typ.

```csharp
public OperatorType Operator { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormatConditionPropertyOperatorDemo
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
            
            // Lägg till villkorsstyrd formatering
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];
            
            // Skapa cellområde
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 2;
            area.EndColumn = 0;
            
            // Lägg till villkor
            int conditionIndex = fcc.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "15", "25");
            FormatCondition fc = fcc[conditionIndex];
            
            // Ställ in stil
            Style style = workbook.CreateStyle();
            style.Font.Color = System.Drawing.Color.Red;
            fc.Style = style;
            
            // Demonstrera användning av egenskapen Operator
            Console.WriteLine("Operator Type: " + fc.Operator);
            if (fc.Operator == OperatorType.Between)
            {
                Console.WriteLine("Condition is set to BETWEEN values");
            }
            
            // Spara arbetsboken
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* enum [OperatorType](../../operatortype/)
* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



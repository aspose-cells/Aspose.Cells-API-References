---
title: "FormatCondition.StopIfTrue"
second_title: "Aspose.Cells för .NET API‑referens"
description: "FormatCondition property. När detta är sant får inga regler med lägre prioritet tillämpas över denna regel när regeln utvärderas till sant. Gäller endast för Excel 2007"
type: docs
url: /sv/net/aspose.cells/formatcondition/stopiftrue/
---
## FormatCondition.StopIfTrue property

Sant, inga regler med lägre prioritet får tillämpas över denna regel när den utvärderas till sant. Gäller endast för Excel 2007;

```csharp
public bool StopIfTrue { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormatConditionPropertyStopIfTrueDemo
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
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
            
            // Lägg till villkor och sätt StopIfTrue
            int conditionIndex = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "15", "35");
            FormatCondition condition = fcs[conditionIndex];
            condition.StopIfTrue = true;
            
            // Lägg till ett annat villkor som normalt skulle åsidosätta det första
            int conditionIndex2 = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.GreaterThan, "25", "");
            FormatCondition condition2 = fcs[conditionIndex2];
            condition2.StopIfTrue = false;

            // Spara arbetsboken
            workbook.Save("StopIfTrueDemo.xlsx");
        }
    }
}
```

### Se även

* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



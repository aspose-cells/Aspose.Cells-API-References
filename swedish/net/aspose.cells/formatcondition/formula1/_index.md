---
title: "FormatCondition.Formula1"
second_title: "Aspose.Cells för .NET API‑referens"
description: "FormatCondition-egenskap. Hämtar och anger värdet eller uttrycket som är kopplat till villkorlig formatering"
type: docs
url: /sv/net/aspose.cells/formatcondition/formula1/
---
## FormatCondition.Formula1 property

Hämtar och anger värdet eller uttrycket som är kopplat till villkorlig formatering.

```csharp
public string Formula1 { get; set; }
```

### Anmärkningar

Lägg till alla områden innan du anger formeln. För att ange formel för detta villkor, om inmatningsvärdet börjar med '=', kommer det att behandlas som en formel. Annars behandlas det som ett vanligt värde (text, tal, bool). För textvärden som börjar med '=', kan användaren ange det som formel i formatet: \"=\\\"=...\\\"\".

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormatConditionPropertyFormula1Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            worksheet.Cells["E1"].PutValue(50);
            
            // Lägg till villkorsstyrd formatering
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];
            
            // Ange intervallet och villkorstypen
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 5;
            area.EndColumn = 5;
            fcc.AddCondition(FormatConditionType.CellValue, OperatorType.LessOrEqual, "=$E$1<=100", null);
            
            // Kom åt och visa Formula1‑egenskapen
            FormatCondition fc = fcc[0];
            Console.WriteLine("Formula1: " + fc.Formula1);
        }
    }
}
```

### Se även

* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



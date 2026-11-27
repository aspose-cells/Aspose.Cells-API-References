---
title: "FormatCondition.Formula2"
second_title: "Aspose.Cells för .NET API‑referens"
description: "FormatCondition-egenskap. Hämtar och anger värdet eller uttrycket som är kopplat till villkorlig formatering"
type: docs
url: /sv/net/aspose.cells/formatcondition/formula2/
---
## FormatCondition.Formula2 property

Hämtar och anger värdet eller uttrycket som är kopplat till villkorlig formatering.

```csharp
public string Formula2 { get; set; }
```

### Anmärkningar

Lägg till alla områden innan du anger formeln. För att ange formel för detta villkor, om inmatningsvärdet börjar med '=', kommer det att behandlas som en formel. Annars behandlas det som ett vanligt värde (text, tal, bool). För textvärden som börjar med '=', kan användaren ange det som formel i formatet: \"=\\\"=...\\\"\".

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormatConditionPropertyFormula2Demo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till villkorsstyrd formatering
            ConditionalFormattingCollection conditionalFormattings = worksheet.ConditionalFormattings;
            int index = conditionalFormattings.Add();
            FormatConditionCollection formatConditions = conditionalFormattings[index];
            
            // Definiera cellintervallet
            CellArea area = CellArea.CreateCellArea(0, 0, 1, 1);
            
            // Lägg till formatvillkor med Formula2
            formatConditions.Add(area, 
                FormatConditionType.CellValue, 
                OperatorType.Between, 
                "=\"abc def\"", 
                "=\"a\"&\"b\"");

            // Hämta formatvillkoret
            FormatCondition formatCondition = formatConditions[0];

            // Skriv ut formlerna
            Console.WriteLine("Formula1: " + formatCondition.Formula1);
            Console.WriteLine("Formula2: " + formatCondition.Formula2);

            // Spara arbetsboken
            workbook.Save("FormatConditionFormula2Demo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Se även

* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



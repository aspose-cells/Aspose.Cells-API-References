---
title: "FormatConditionCollection.Item"
second_title: "Aspose.Cells för .NET API‑referens"
description: "FormatConditionCollection egenskap. Hämtar formateringsvillkoret med index"
type: docs
url: /sv/net/aspose.cells/formatconditioncollection/item/
---
## FormatConditionCollection indexer

Hämtar formateringsvillkoret efter index.

```csharp
public FormatCondition this[int index] { get; }
```

| Parameter | Beskrivning |
| --- | --- |
| index | indexet för det formateringsvillkor som ska returneras. |

### Returvärde

formateringsvillkoret

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormatConditionCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till en formatvillkorssamling
            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = sheet.ConditionalFormattings[index];
            
            // Lägg till ett formatvillkor
            fcc.Add(CellArea.CreateCellArea(0, 0, 0, 3),
                FormatConditionType.CellValue, OperatorType.Between, "=A1", "=B1");

            // Åtkomst till det första formatvillkoret med Item-egenskapen
            FormatCondition condition = fcc[0];
            
            // Visa formlerna
            Console.WriteLine("Formula1: " + condition.Formula1);
            Console.WriteLine("Formula2: " + condition.Formula2);
            
            // Ändra formlerna med Item-egenskapen
            fcc[0].Formula1 = "=C1";
            fcc[0].Formula2 = "=D1";
            
            // Visa ändrade formler
            Console.WriteLine("Modified Formula1: " + fcc[0].Formula1);
            Console.WriteLine("Modified Formula2: " + fcc[0].Formula2);
        }
    }
}
```

### Se även

* class [FormatCondition](../../formatcondition/)
* class [FormatConditionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



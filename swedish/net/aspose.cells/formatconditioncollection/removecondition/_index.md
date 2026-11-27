---
title: "FormatConditionCollection.RemoveCondition"
second_title: "Aspose.Cells för .NET API‑referens"
description: "FormatConditionCollection metod. Tar bort formateringsvillkoret med index"
type: docs
url: /sv/net/aspose.cells/formatconditioncollection/removecondition/
---
## FormatConditionCollection.RemoveCondition method

Tar bort formateringsvillkoret efter index.

```csharp
public void RemoveCondition(int index)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | Int32 | Index för det formateringsvillkor som ska tas bort. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FormatConditionCollectionMethodRemoveConditionWithInt32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Hämta samlingen av formatvillkor
            FormatConditionCollection formatConditions = worksheet.ConditionalFormattings[0];
            
            // Lägg till några exempelvillkor
            int index1 = formatConditions.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "10", "100");
            int index2 = formatConditions.AddCondition(FormatConditionType.CellValue, OperatorType.GreaterThan, "50", "");
            
            try
            {
                // Visa initialt antal
                Console.WriteLine($"Initial conditions count: {formatConditions.Count}");
                
                // Ta bort det första villkoret
                formatConditions.RemoveCondition(index1);
                
                // Visa uppdaterat antal
                Console.WriteLine($"Conditions count after removal: {formatConditions.Count}");
                
                // Spara arbetsboken
                workbook.Save("RemoveConditionDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling RemoveCondition: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [FormatConditionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



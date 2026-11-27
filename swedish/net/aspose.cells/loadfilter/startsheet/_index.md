---
title: "LoadFilter.StartSheet"
second_title: "Aspose.Cells för .NET API‑referens"
description: "LoadFilter-metod. Förbereder filteralternativ innan det givna kalkylbladet laddas. Användares implementation av LoadFilter kan ändra LoadDataFilterOptions här för att ange hur data ska laddas för detta kalkylblad."
type: docs
url: /sv/net/aspose.cells/loadfilter/startsheet/
---
## LoadFilter.StartSheet method

Förbereder filteralternativ innan det angivna kalkylbladet läses in. Användarens implementation av LoadFilter kan ändra LoadDataFilterOptions här för att ange hur data ska läsas in för detta kalkylblad.

```csharp
public virtual void StartSheet(Worksheet sheet)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| blad | Arbetsblad | Arbetsbladet som ska laddas. Det finns bara några få egenskaper som kan användas för det givna arbetsbladsobjektet här eftersom de flesta data och egenskaper inte har laddats. De tillgängliga egenskaperna är: Name, Index, VisibilityType |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class LoadFilterMethodStartSheetWithWorksheetDemo
    {
        // Skapa en anpassad laddningsfilterklass som ärver LoadFilter
        class CustomLoadFilter : LoadFilter
        {
            public override void StartSheet(Worksheet sheet)
            {
                Console.WriteLine($"Processing sheet: {sheet.Name}");
                // Du kan lägga till anpassad logik här för att hantera specifika blad
            }
        }

        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Name = "TestSheet";

            // Skapa en instans av vårt anpassade laddningsfilter
            CustomLoadFilter loadFilter = new CustomLoadFilter();

            try
            {
                // Anropa StartSheet‑metoden med arbetsbladsparametern
                loadFilter.StartSheet(worksheet);
                
                Console.WriteLine("StartSheet method executed successfully");
                
                // Lägg till lite data för att demonstrera att bladet är åtkomligt
                worksheet.Cells["A1"].PutValue("StartSheet Demo");
                worksheet.Cells["A2"].PutValue(DateTime.Now.ToString());
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing StartSheet method: {ex.Message}");
            }
            
            // Spara resultatet
            workbook.Save("LoadFilterStartSheetDemo.xlsx");
        }
    }
}
```

### Se även

* class [Worksheet](../../worksheet/)
* class [LoadFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



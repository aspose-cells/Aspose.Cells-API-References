---
title: "Klass PowerQueryFormulaItem"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.QueryTables.PowerQueryFormulaItem‑klass. Representerar objektet för power query‑formeln"
type: docs
url: /sv/net/aspose.cells.querytables/powerqueryformulaitem/
---
## PowerQueryFormulaItem class

Representerar elementet i Power Query‑formeln.

```csharp
public class PowerQueryFormulaItem
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [ItemType](../../aspose.cells.querytables/powerqueryformulaitem/itemtype/) { get; } | Hämtar typen för detta objekt (Function, Parameter, List, Literal eller Unknown). |
| [Name](../../aspose.cells.querytables/powerqueryformulaitem/name/) { get; } | Hämtar namnet på objektet. |
| [TextValue](../../aspose.cells.querytables/powerqueryformulaitem/textvalue/) { get; } | Hämtar textvärdet för objektet. |
| [Value](../../aspose.cells.querytables/powerqueryformulaitem/value/) { get; set; } | Hämtar värdet för objektet. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using System;
    using Aspose.Cells;
    using Aspose.Cells.QueryTables;

    public class QueryTablesClassPowerQueryFormulaItemDemo
    {
        public static void Run()
        {
            try
            {
                // Skapa en ny arbetsbok (kan vara en befintlig fil om du har Power Query‑data)
                Workbook workbook = new Workbook();

                // Få åtkomst till DataMashup‑objektet som innehåller PowerQuery‑formler
                DataMashup mashup = workbook.DataMashup;

                bool itemFound = false;

                // Iterera genom alla PowerQuery‑formler och deras objekt
                foreach (PowerQueryFormula formula in mashup.PowerQueryFormulas)
                {
                    foreach (PowerQueryFormulaItem item in formula.PowerQueryFormulaItems)
                    {
                        // Demonstrera skrivskyddad Name‑egenskap
                        Console.WriteLine($"Item Name: {item.Name}");

                        // Demonstrera läs/skriv Value‑egenskap
                        Console.WriteLine($"Original Value: {item.Value}");
                        item.Value = "SampleValue";
                        Console.WriteLine($"Modified Value: {item.Value}");

                        itemFound = true;
                    }
                }

                if (!itemFound)
                {
                    Console.WriteLine("No PowerQueryFormulaItem instances were found in the workbook.");
                }

                Console.WriteLine("PowerQueryFormulaItem demo completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with PowerQueryFormulaItem: {ex.Message}");
            }
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.QueryTables](../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../)



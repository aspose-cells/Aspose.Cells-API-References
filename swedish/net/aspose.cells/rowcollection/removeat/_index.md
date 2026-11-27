---
title: "RowCollection.RemoveAt"
second_title: "Aspose.Cells för .NET API‑referens"
description: "RowCollection‑metod. Ta bort radobjektet på den specificerade indexpositionen i denna samling"
type: docs
url: /sv/net/aspose.cells/rowcollection/removeat/
---
## RowCollection.RemoveAt method

Ta bort radobjektet på det angivna indexet (positionen) i denna samling.

```csharp
public void RemoveAt(int index)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | Int32 | nollbaserat index (position, inte [`Index`](../../row/index/)) för det befintliga radobjektet i denna samling. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class RowCollectionMethodRemoveAtWithInt32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till data i celler i de första raderna
            worksheet.Cells["A1"].PutValue("Row 1");
            worksheet.Cells["A2"].PutValue("Row 2");
            worksheet.Cells["A3"].PutValue("Row 3");
            worksheet.Cells["A4"].PutValue("Row 4");

            // Visa initial radantal
            Console.WriteLine($"Initial row count: {worksheet.Cells.Rows.Count}");

            try
            {
                // Anropa RemoveAt‑metoden för att ta bort raden på index 1 (andra raden)
                worksheet.Cells.Rows.RemoveAt(1);

                Console.WriteLine("Method executed successfully. Row at index 1 removed.");

                // Visa uppdaterat radantal
                Console.WriteLine($"Updated row count: {worksheet.Cells.Rows.Count}");

                // Visa effekten – Rad 2 ska tas bort, Rad 3 blir Rad 2
                Console.WriteLine("Cell A1: " + worksheet.Cells["A1"].StringValue);
                Console.WriteLine("Cell A2: " + worksheet.Cells["A2"].StringValue);
                Console.WriteLine("Cell A3: " + worksheet.Cells["A3"].StringValue);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing RemoveAt method: {ex.Message}");
            }

            // Spara resultatet
            workbook.Save("RowCollectionMethodRemoveAtWithInt32Demo.xlsx");
        }
    }
}
```

### Se även

* class [RowCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



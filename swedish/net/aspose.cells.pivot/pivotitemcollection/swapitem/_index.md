---
title: "PivotItemCollection.SwapItem"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotItemCollection-metod. Byt direkt två items"
type: docs
url: /sv/net/aspose.cells.pivot/pivotitemcollection/swapitem/
---
## PivotItemCollection.SwapItem method

Byt direkt plats på två objekt.

```csharp
public void SwapItem(int index1, int index2)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index1 | Int32 |  |
| index2 | Int32 |  |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotItemCollectionMethodSwapItemWithInt32Int32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för pivottabell
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["B3"].Value = 200;
            worksheet.Cells["B4"].Value = 300;

            // Skapa pivottabell
            int index = worksheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");

            // Hämta pivotelement
            PivotField pivotField = pivotTable.RowFields[0];
            PivotItemCollection pivotItems = pivotField.PivotItems;

            try
            {
                // Visa ursprunglig ordning
                Console.WriteLine("Original order:");
                foreach (PivotItem item in pivotItems)
                {
                    Console.WriteLine(item.Name);
                }

                // Byt plats på element vid index 0 och 1
                pivotItems.SwapItem(0, 1);

                // Visa ny ordning
                Console.WriteLine("\nAfter swapping:");
                foreach (PivotItem item in pivotItems)
                {
                    Console.WriteLine(item.Name);
                }

                Console.WriteLine("SwapItem method executed successfully with parameters (0, 1)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SwapItem method: {ex.Message}");
            }

            // Spara resultatet
            workbook.Save("PivotItemCollectionMethodSwapItemWithInt32Int32Demo.xlsx");
        }
    }
}
```

### Se även

* class [PivotItemCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)



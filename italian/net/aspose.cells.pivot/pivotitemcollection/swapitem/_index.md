---
title: "PivotItemCollection.SwapItem"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "PivotItemCollection method. Scambia direttamente due elementi"
type: docs
url: /it/net/aspose.cells.pivot/pivotitemcollection/swapitem/
---
## PivotItemCollection.SwapItem method

Scambia direttamente due elementi.

```csharp
public void SwapItem(int index1, int index2)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| index1 | Int32 |  |
| index2 | Int32 |  |

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per la tabella pivot
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["B3"].Value = 200;
            worksheet.Cells["B4"].Value = 300;

            // Crea tabella pivot
            int index = worksheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");

            // Ottieni gli elementi pivot
            PivotField pivotField = pivotTable.RowFields[0];
            PivotItemCollection pivotItems = pivotField.PivotItems;

            try
            {
                // Mostra l'ordine originale
                Console.WriteLine("Original order:");
                foreach (PivotItem item in pivotItems)
                {
                    Console.WriteLine(item.Name);
                }

                // Scambia gli elementi agli indici 0 e 1
                pivotItems.SwapItem(0, 1);

                // Mostra il nuovo ordine
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

            // Salva il risultato
            workbook.Save("PivotItemCollectionMethodSwapItemWithInt32Int32Demo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotItemCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)



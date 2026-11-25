---
title: "PivotItemCollection.ChangeitemsOrder"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "PivotItemCollection method. Modifica direttamente l'ordine dei due elementi"
type: docs
url: /it/net/aspose.cells.pivot/pivotitemcollection/changeitemsorder/
---
## PivotItemCollection.ChangeitemsOrder method

Modifica direttamente l'ordine dei due elementi.

```csharp
[Obsolete("Use PivotItemCollection.SwapItem() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void ChangeitemsOrder(int sourceIndex, int destIndex)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sourceIndex | Int32 | L'indice corrente |
| destIndex | Int32 | L'indice di destinazione |

### Osservazioni

NOTA: Questo metodo è ora obsoleto. Invece, si prega di utilizzare il metodo PivotItemCollection.SwapItem(). Questo metodo sarà rimosso 12 mesi dopo, a partire da luglio 2024. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotItemCollectionMethodChangeitemsOrderWithInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            worksheet.Cells[0, 0].Value = "Category";
            worksheet.Cells[1, 0].Value = "A";
            worksheet.Cells[2, 0].Value = "B";
            worksheet.Cells[3, 0].Value = "C";

            PivotTableCollection pivotTables = worksheet.PivotTables;
            int pivotIndex = pivotTables.Add("=Sheet1!A1:A4", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[pivotIndex];

            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            PivotField pivotField = pivotTable.RowFields[0];
            PivotItemCollection pivotItems = pivotField.PivotItems;

            Console.WriteLine("Original Order:");
            foreach (PivotItem item in pivotItems)
            {
                Console.WriteLine(item.Name);
            }

            pivotItems.ChangeitemsOrder(0, 2);

            Console.WriteLine("\nAfter Changing Order:");
            foreach (PivotItem item in pivotItems)
            {
                Console.WriteLine(item.Name);
            }

            workbook.Save("PivotItemOrderChange.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotItemCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)



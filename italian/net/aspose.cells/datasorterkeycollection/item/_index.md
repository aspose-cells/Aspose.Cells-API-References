---
title: "DataSorterKeyCollection.Item"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà DataSorterKeyCollection. Ottiene e imposta DataSorterKey per indice"
type: docs
url: /it/net/aspose.cells/datasorterkeycollection/item/
---
## DataSorterKeyCollection indexer

Ottiene e imposta [`DataSorterKey`](../../datasorterkey/) per indice.

```csharp
public DataSorterKey this[int index] { get; }
```

| Parametro | Descrizione |
| --- | --- |
| indice | L'indice. |

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class DataSorterKeyCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["A4"].PutValue("Bob");
            worksheet.Cells["B1"].PutValue("Score");
            worksheet.Cells["B2"].PutValue(85);
            worksheet.Cells["B3"].PutValue(92);
            worksheet.Cells["B4"].PutValue(78);

            // Crea un oggetto lista (tabella)
            int index = worksheet.ListObjects.Add(0, 0, 3, 1, true);
            ListObject table = worksheet.ListObjects[index];

            // Aggiungi chiave di ordinamento (ordina per colonna Score in ordine decrescente)
            table.AutoFilter.Sorter.AddKey(1, SortOrder.Descending);
            table.AutoFilter.Sorter.Sort();

            // Dimostra l'uso della proprietà Item
            DataSorterKey key = table.AutoFilter.Sorter.Keys[0];
            Console.WriteLine("Sort Key Index: {0}, Order: {1}", key.Index, key.Order);

            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [DataSorterKey](../../datasorterkey/)
* class [DataSorterKeyCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



---
title: "DataSorter.Keys"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà DataSorter. Ottiene l'elenco delle chiavi del DataSorter"
type: docs
url: /it/net/aspose.cells/datasorter/keys/
---
## DataSorter.Keys property

Restituisce l'elenco delle chiavi del data sorter.

```csharp
public DataSorterKeyCollection Keys { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterPropertyKeysDemo
    {
        public static void Run()
        {
            // Crea un oggetto cartella di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("USA");
            worksheet.Cells["A2"].PutValue("China");
            worksheet.Cells["A3"].PutValue("Brazil");
            worksheet.Cells["A4"].PutValue("Russia");
            worksheet.Cells["A5"].PutValue("Canada");

            // Inizializza DataSorter
            DataSorter sorter = workbook.DataSorter;
            
            // Aggiungi chiave di ordinamento per la colonna A (indice 0)
            sorter.AddKey(0, SortOrder.Ascending);

            // Ordina i dati
            sorter.Sort(worksheet.Cells, CellArea.CreateCellArea("A1", "A5"));

            // Dimostra l'uso della proprietà Keys
            DataSorterKeyCollection keys = sorter.Keys;
            Console.WriteLine("Sort Keys Information:");
            foreach (DataSorterKey key in keys)
            {
                Console.WriteLine($"Column Index: {key.Index}, Sort Order: {key.Order}");
            }

            // Salva la cartella di lavoro
            workbook.Save("DataSorterKeysDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [DataSorterKeyCollection](../../datasorterkeycollection/)
* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



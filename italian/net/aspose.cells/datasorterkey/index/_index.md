---
title: "DataSorterKey.Index"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà DataSorterKey. Ottiene l'indice della colonna ordinata, posizione assoluta: la colonna A è 0, B è 1"
type: docs
url: /it/net/aspose.cells/datasorterkey/index/
---
## DataSorterKey.Index property

Ottiene l'indice della colonna ordinata (posizione assoluta, la colonna A è 0, B è 1, ...).

```csharp
public int Index { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterKeyPropertyIndexDemo
    {
        public static void Run()
        {
            // Crea un oggetto cartella di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio da ordinare
            worksheet.Cells["A1"].PutValue("USA");
            worksheet.Cells["A2"].PutValue("China");
            worksheet.Cells["A3"].PutValue("Brazil");
            worksheet.Cells["A4"].PutValue("Russia");
            worksheet.Cells["A5"].PutValue("Canada");

            // Crea un ordinatore di dati e aggiungi la chiave di ordinamento
            DataSorter sorter = workbook.DataSorter;
            sorter.AddKey(0, SortOrder.Ascending);

            // Ordina i dati
            CellArea ca = CellArea.CreateCellArea("A1", "A5");
            sorter.Sort(worksheet.Cells, ca);

            // Dimostra l'uso della proprietà Index
            foreach (DataSorterKey key in sorter.Keys)
            {
                Console.WriteLine($"Column index being sorted: {key.Index}");
            }

            // Salva il risultato
            workbook.Save("DataSorterKeyExample.xlsx");
        }
    }
}
```

### Vedi anche

* class [DataSorterKey](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



---
title: "DataSorterKey.Type"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà DataSorterKey. Rappresenta il tipo di ordinamento"
type: docs
url: /it/net/aspose.cells/datasorterkey/type/
---
## DataSorterKey.Type property

Rappresenta il tipo di ordinamento.

```csharp
public SortOnType Type { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterKeyPropertyTypeDemo
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

            // Crea un ordinatore di dati e aggiungi la chiave
            DataSorter sorter = workbook.DataSorter;
            sorter.AddKey(0, SortOrder.Ascending);

            // Ordina i dati
            CellArea ca = CellArea.CreateCellArea("A1", "A5");
            sorter.Sort(worksheet.Cells, ca);

            // Dimostra l'uso della proprietà Type
            foreach (DataSorterKey key in sorter.Keys)
            {
                Console.WriteLine($"Key Type: {key.Type}");
            }
        }
    }
}
```

### Vedi anche

* enum [SortOnType](../../sortontype/)
* class [DataSorterKey](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



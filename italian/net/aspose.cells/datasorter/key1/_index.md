---
title: "DataSorter.Key1"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà DataSorter. Rappresenta l'indice della prima colonna ordinata, posizione assoluta: la colonna A è 0, B è 1"
type: docs
url: /it/net/aspose.cells/datasorter/key1/
---
## DataSorter.Key1 property

Rappresenta l'indice della prima colonna ordinata (posizione assoluta, la colonna A è 0, B è 1, ...).

```csharp
public int Key1 { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterPropertyKey1Demo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro e aggiungi dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Aggiungi dati di esempio
            cells["A1"].PutValue("Name");
            cells["B1"].PutValue("Score");
            cells["A2"].PutValue("John");
            cells["B2"].PutValue(85);
            cells["A3"].PutValue("Alice");
            cells["B3"].PutValue(92);
            cells["A4"].PutValue("Bob");
            cells["B4"].PutValue(78);

            // Crea un ordinatore di dati e imposta Key1 per ordinare per la colonna Score (colonna B)
            DataSorter sorter = workbook.DataSorter;
            sorter.Key1 = 1; // Column index 1 (B)
            sorter.Order1 = SortOrder.Descending;

            // Definisci l'area di ordinamento (righe 1-4, tutte le colonne dei dati)
            CellArea sortArea = new CellArea();
            sortArea.StartRow = 1;
            sortArea.EndRow = 4;
            sortArea.StartColumn = 0;
            sortArea.EndColumn = cells.MaxDataColumn;

            // Esegui l'ordinamento
            sorter.Sort(cells, sortArea);

            // Salva il risultato
            workbook.Save("SortedData.xlsx");
        }
    }
}
```

### Vedi anche

* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



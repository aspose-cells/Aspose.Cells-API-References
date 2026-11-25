---
title: "DataSorter.HasHeaders"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà DataSorter. Rappresenta se l'intervallo ha intestazioni"
type: docs
url: /it/net/aspose.cells/datasorter/hasheaders/
---
## DataSorter.HasHeaders property

Rappresenta se l'intervallo ha intestazioni.

```csharp
public bool HasHeaders { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterPropertyHasHeadersDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi intestazioni e dati di esempio
            worksheet.Cells["A1"].PutValue("Fruits");
            worksheet.Cells["B1"].PutValue("Quantity");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["B2"].PutValue(15);
            worksheet.Cells["B3"].PutValue(8);
            worksheet.Cells["B4"].PutValue(12);

            // Crea DataSorter e imposta HasHeaders su true
            DataSorter sorter = workbook.DataSorter;
            sorter.HasHeaders = true; // This tells the sorter the first row contains headers
            
            // Ordina per la prima colonna (Frutta) in ordine crescente
            sorter.AddKey(0, SortOrder.Ascending);
            
            // Ordina l'intervallo di dati (incluse le intestazioni)
            sorter.Sort(worksheet.Cells, CellArea.CreateCellArea("A1", "B4"));

            // Salva la cartella di lavoro ordinata
            workbook.Save("SortedWithHeaders.xlsx");
        }
    }
}
```

### Vedi anche

* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



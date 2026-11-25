---
title: "DataSorter.Order1"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà DataSorter. Rappresenta l'ordine di ordinamento della prima chiave"
type: docs
url: /it/net/aspose.cells/datasorter/order1/
---
## DataSorter.Order1 property

Rappresenta l'ordine di ordinamento della prima chiave.

```csharp
public SortOrder Order1 { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterPropertyOrder1Demo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Score");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(85);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(92);
            worksheet.Cells["A4"].PutValue("Bob");
            worksheet.Cells["B4"].PutValue(78);

            // Imposta le proprietà dell'ordinatore dei dati
            DataSorter sorter = workbook.DataSorter;
            sorter.Order1 = SortOrder.Ascending;
            sorter.Key1 = 1; // Sort by column B (Score)
            
            // Definisci l'intervallo di ordinamento
            CellArea area = CellArea.CreateCellArea("A1", "B4");
            
            // Esegui l'ordinamento
            sorter.Sort(worksheet.Cells, area);
            
            // Salva la cartella di lavoro
            workbook.Save("SortedOutput.xlsx");
        }
    }
}
```

### Vedi anche

* enum [SortOrder](../../sortorder/)
* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



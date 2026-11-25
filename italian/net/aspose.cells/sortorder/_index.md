---
title: "Enum SortOrder"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Enum Aspose.Cells.SortOrder. Rappresenta l'ordine di ordinamento per l'intervallo di dati"
type: docs
url: /it/net/aspose.cells/sortorder/
---
## SortOrder enumeration

Rappresenta l'ordine di ordinamento per l'intervallo di dati.

```csharp
public enum SortOrder
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Ascending | `0` | Ordina i dati in ordine crescente |
| Descending | `1` | Ordina i dati in ordine decrescente |
| Natural | `2` | Mantiene l'ordine originale dei dati senza ordinamento. Si applica solo a scenari speciali come PivotTable. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassSortOrderDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            var workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio da ordinare
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Score");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(85);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(92);
            worksheet.Cells["A4"].PutValue("Bob");
            worksheet.Cells["B4"].PutValue(78);
            
            // Crea un ordinatore di dati
            var sorter = workbook.DataSorter;
            
            // Imposta l'ordine di ordinamento e le chiavi
            sorter.Order1 = SortOrder.Descending;
            sorter.Key1 = 1; // Sort by column B (Score)
            
            // Definisci area di ordinamento
            var sortArea = new CellArea
            {
                StartRow = 0,
                StartColumn = 0,
                EndRow = 3,
                EndColumn = 1
            };
            
            // Esegui l'ordinamento
            sorter.Sort(worksheet.Cells, sortArea);
            
            // Salva la cartella di lavoro
            workbook.Save("SortedData.xlsx");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)



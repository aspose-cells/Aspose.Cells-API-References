---
title: "Enum SortOnType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Enum Aspose.Cells.SortOnType. Tipo di valore ordinato"
type: docs
url: /it/net/aspose.cells/sortontype/
---
## SortOnType enumeration

Tipo di valore ordinato.

```csharp
public enum SortOnType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Value | `0` | Ordina per valore delle celle. |
| CellColor | `1` | Ordina per colore delle celle. |
| FontColor | `2` | Ordina per colore del carattere delle celle. |
| Icon | `3` | Ordina per icona condizionale. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SortOnTypeDemo
    {
        public static void SortOnTypeExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Aggiungi un nuovo foglio di lavoro alla cartella di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio al foglio di lavoro
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["A3"].PutValue("Jane");
            worksheet.Cells["A4"].PutValue("Doe");

            worksheet.Cells["B1"].PutValue("Score");
            worksheet.Cells["B2"].PutValue(85);
            worksheet.Cells["B3"].PutValue(95);
            worksheet.Cells["B4"].PutValue(75);

            // Applica il filtro automatico all'intervallo
            worksheet.AutoFilter.Range = "A1:B4";

            // Ottieni il filtro automatico
            AutoFilter autoFilter = worksheet.AutoFilter;

            // Ottieni l'ordinatore dei dati
            DataSorter sorter = autoFilter.Sorter;

            // Imposta la prima chiave per ordinare per i valori nella seconda colonna (Score)
            sorter.AddKey(1, SortOnType.Value, SortOrder.Descending, null);

            // Ordina i dati nell'intervallo
            sorter.Sort(worksheet.Cells, 1, 0, 3, 1);

            // Salva la cartella di lavoro
            workbook.Save("SortOnTypeExample.xlsx");

            // Restituisci i risultati
            Console.WriteLine("Data sorted by Score in descending order.");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)



---
title: "Classe DataSorter"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.DataSorter. Descrizione sommaria per DataSorter"
type: docs
url: /it/net/aspose.cells/datasorter/
---
## DataSorter class

Descrizione sommaria per DataSorter.

```csharp
public class DataSorter
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [CaseSensitive](../../aspose.cells/datasorter/casesensitive/) { get; set; } | Ottiene e imposta se la distinzione tra maiuscole e minuscole è attiva durante il confronto di stringhe. |
| [HasHeaders](../../aspose.cells/datasorter/hasheaders/) { get; set; } | Rappresenta se l'intervallo ha intestazioni. |
| [Key1](../../aspose.cells/datasorter/key1/) { get; set; } | Rappresenta l'indice della prima colonna ordinata (posizione assoluta, la colonna A è 0, B è 1, ...). |
| [Key2](../../aspose.cells/datasorter/key2/) { get; set; } | Rappresenta l'indice della seconda colonna ordinata (posizione assoluta, la colonna A è 0, B è 1, ...). |
| [Key3](../../aspose.cells/datasorter/key3/) { get; set; } | Rappresenta l'indice della terza colonna ordinata (posizione assoluta, la colonna A è 0, B è 1, ...). |
| [Keys](../../aspose.cells/datasorter/keys/) { get; } | Restituisce l'elenco delle chiavi del data sorter. |
| [Order1](../../aspose.cells/datasorter/order1/) { get; set; } | Rappresenta l'ordine di ordinamento della prima chiave. |
| [Order2](../../aspose.cells/datasorter/order2/) { get; set; } | Rappresenta l'ordine di ordinamento della seconda chiave. |
| [Order3](../../aspose.cells/datasorter/order3/) { get; set; } | Rappresenta l'ordine di ordinamento della terza chiave. |
| [SortAsNumber](../../aspose.cells/datasorter/sortasnumber/) { get; set; } | Indica se ordinare elementi che sembrano numeri. |
| [SortLeftToRight](../../aspose.cells/datasorter/sortlefttoright/) { get; set; } | True indica che l'orientamento dell'ordinamento è da sinistra a destra. False indica che l'orientamento dell'ordinamento è dall'alto verso il basso. Il valore predefinito è false. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [AddColorKey](../../aspose.cells/datasorter/addcolorkey/)(int, SortOnType, SortOrder, Color) | Aggiunge una chiave di ordinamento per colore. |
| [AddKey](../../aspose.cells/datasorter/addkey/#addkey_1)(int, SortOrder) | Aggiunge l'indice della colonna ordinata e l'ordine di ordinamento. |
| [AddKey](../../aspose.cells/datasorter/addkey/#addkey_2)(int, SortOrder, string) | Aggiunge l'indice di colonna ordinata e l'ordine di ordinamento con un elenco di ordinamento personalizzato. |
| [AddKey](../../aspose.cells/datasorter/addkey/#addkey_3)(int, SortOrder, string[]) | Aggiunge l'indice di colonna ordinata e l'ordine di ordinamento con un elenco di ordinamento personalizzato. |
| [AddKey](../../aspose.cells/datasorter/addkey/#addkey)(int, SortOnType, SortOrder, object) | Aggiunge l'indice di colonna ordinata e l'ordine di ordinamento con un elenco di ordinamento personalizzato. |
| [Clear](../../aspose.cells/datasorter/clear/)() | Cancella tutte le impostazioni. |
| [Sort](../../aspose.cells/datasorter/sort/#sort)() | Ordina i dati nell'intervallo. |
| [Sort](../../aspose.cells/datasorter/sort/#sort_1)(Cells, CellArea) | Ordina i dati dell'area. |
| [Sort](../../aspose.cells/datasorter/sort/#sort_2)(Cells, int, int, int, int) | Ordina i dati dell'area. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DataSorterDemo
    {
        public static void DataSorterExample()
        {
            // Istanzia un nuovo oggetto Workbook
            Workbook workbook = new Workbook("DataSorter_original.xlsx");

            // Ottieni l'oggetto DataSorter del workbook
            DataSorter sorter = workbook.DataSorter;

            // Imposta il primo ordine per l'oggetto DataSorter
            sorter.Order1 = SortOrder.Descending;
            // Definisci la prima chiave
            sorter.Key1 = 0;

            // Imposta il secondo ordine per l'oggetto DataSorter
            sorter.Order2 = SortOrder.Ascending;
            // Definisci la seconda chiave
            sorter.Key2 = 1;

            // Crea un'area di celle (intervallo)
            CellArea ca = new CellArea
            {
                StartRow = 0,
                StartColumn = 0,
                EndRow = 13,
                EndColumn = 1
            };

            // Ordina i dati nell'intervallo di dati specificato (A1:B14)
            sorter.Sort(workbook.Worksheets[0].Cells, ca);

            // Salva il file Excel
            workbook.Save("DataSorterExample.xlsx");
            workbook.Save("DataSorterExample.pdf");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)



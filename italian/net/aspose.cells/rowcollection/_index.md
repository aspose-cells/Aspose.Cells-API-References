---
title: "Classe RowCollection"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.RowCollection. Raccoglie gli oggetti Row che rappresentano le righe individuali in un foglio di lavoro"
type: docs
url: /it/net/aspose.cells/rowcollection/
---
## RowCollection class

Raccoglie gli oggetti [`Row`](../row/) che rappresentano le righe individuali in un foglio di lavoro.

```csharp
public class RowCollection : IEnumerable
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Count](../../aspose.cells/rowcollection/count/) { get; } | Restituisce il numero di righe in questa raccolta. |
| [Item](../../aspose.cells/rowcollection/item/) { get; } | Restituisce un oggetto [`Row`](../row/) dato l'indice di riga. L'oggetto Row dell'indice specificato verrà istanziato se non esiste già. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Clear](../../aspose.cells/rowcollection/clear/)() | Cancella tutte le righe e le celle. |
| [GetEnumerator](../../aspose.cells/rowcollection/getenumerator/#getenumerator)() | Restituisce un enumeratore che itera le righe attraverso questa raccolta |
| [GetEnumerator](../../aspose.cells/rowcollection/getenumerator/#getenumerator_1)(bool, bool) | Restituisce un enumeratore che itera le righe attraverso questa raccolta |
| [GetRowByIndex](../../aspose.cells/rowcollection/getrowbyindex/)(int) | Restituisce l'oggetto riga in base alla posizione nella lista. |
| [RemoveAt](../../aspose.cells/rowcollection/removeat/)(int) | Rimuove l'elemento riga all'indice (posizione) specificato in questa raccolta. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Collections;

    public class RowCollectionDemo
    {
        public static void RowCollectionExample()
        {
            // Istanziare un oggetto Workbook
            Workbook workbook = new Workbook();

            // Ottenere il riferimento del primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["A2"].PutValue("World");
            worksheet.Cells["A3"].PutValue("Aspose.Cells");
            // Ottieni la raccolta Rows
            RowCollection rows = worksheet.Cells.Rows;

            // Ottieni il numero di righe nella raccolta
            int rowCount = rows.Count;
            Console.WriteLine("Number of rows: " + rowCount);

            // Ottieni la prima riga
            Row firstRow = rows[0];
            Console.WriteLine("First row index: " + firstRow.Index);

            // Itera le righe usando GetEnumerator
            IEnumerator enumerator = rows.GetEnumerator();
            while (enumerator.MoveNext())
            {
                Row row = (Row)enumerator.Current;
                Console.WriteLine("Row index: " + row.Index + ", Height: " + row.Height);
            }

            // Ottieni una riga per indice
            Row specificRow = rows.GetRowByIndex(1);
            Console.WriteLine("Specific row index: " + specificRow.Index);

            // Cancella tutte le righe e le celle
            rows.Clear();
            Console.WriteLine("Rows cleared.");

            // Salva la cartella di lavoro
            workbook.Save("RowCollectionExample.xlsx");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)



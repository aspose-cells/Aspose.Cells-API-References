---
title: "RowCollection.RemoveAt"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo RowCollection. Rimuove l'elemento riga nella posizione indice specificata in questa collezione"
type: docs
url: /it/net/aspose.cells/rowcollection/removeat/
---
## RowCollection.RemoveAt method

Rimuove l'elemento riga all'indice (posizione) specificato in questa raccolta.

```csharp
public void RemoveAt(int index)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| index | Int32 | Indice basato su zero (posizione, non [`Index`](../../row/index/)) dell'elemento riga esistente in questa collezione. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class RowCollectionMethodRemoveAtWithInt32Demo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi alcuni dati alle celle nelle prime righe
            worksheet.Cells["A1"].PutValue("Row 1");
            worksheet.Cells["A2"].PutValue("Row 2");
            worksheet.Cells["A3"].PutValue("Row 3");
            worksheet.Cells["A4"].PutValue("Row 4");

            // Visualizza il conteggio iniziale delle righe
            Console.WriteLine($"Initial row count: {worksheet.Cells.Rows.Count}");

            try
            {
                // Chiama il metodo RemoveAt per rimuovere la riga all'indice 1 (seconda riga)
                worksheet.Cells.Rows.RemoveAt(1);

                Console.WriteLine("Method executed successfully. Row at index 1 removed.");

                // Visualizza il conteggio aggiornato delle righe
                Console.WriteLine($"Updated row count: {worksheet.Cells.Rows.Count}");

                // Mostra l'effetto - La riga 2 dovrebbe essere rimossa, la riga 3 diventa riga 2
                Console.WriteLine("Cell A1: " + worksheet.Cells["A1"].StringValue);
                Console.WriteLine("Cell A2: " + worksheet.Cells["A2"].StringValue);
                Console.WriteLine("Cell A3: " + worksheet.Cells["A3"].StringValue);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing RemoveAt method: {ex.Message}");
            }

            // Salva il risultato
            workbook.Save("RowCollectionMethodRemoveAtWithInt32Demo.xlsx");
        }
    }
}
```

### Vedi anche

* class [RowCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



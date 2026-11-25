---
title: "RowCollection.GetEnumerator"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo RowCollection. Restituisce un enumeratore che itera le righe attraverso questa collezione"
type: docs
url: /it/net/aspose.cells/rowcollection/getenumerator/
---
## GetEnumerator() {#getenumerator}

Restituisce un enumeratore che itera le righe attraverso questa raccolta

```csharp
public IEnumerator GetEnumerator()
```

### Valore di ritorno

L'enumeratore di righe che attraverserà tutte le righe esistenti in questa collezione.

### Esempi

```csharp
using System;
using System.Collections;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowCollectionMethodGetEnumeratorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Imposta le altezze delle righe per la dimostrazione
            worksheet.Cells.SetRowHeight(0, 15);
            worksheet.Cells.SetRowHeight(1, 20);
            worksheet.Cells.SetRowHeight(2, 25);

            IEnumerator enumerator = worksheet.Cells.Rows.GetEnumerator();
            while (enumerator.MoveNext())
            {
                Row row = (Row)enumerator.Current;
                Console.WriteLine($"Row index: {row.Index}, Height: {row.Height}");
            }
        }
    }
}
```

### Vedi anche

* class [RowCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetEnumerator(bool, bool) {#getenumerator_1}

Restituisce un enumeratore che itera le righe attraverso questa raccolta

```csharp
public IEnumerator GetEnumerator(bool reversed, bool sync)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| invertito | Booleano | se enumerare le righe in ordine invertito |
| sync | Booleano | se l'enumeratore restituito deve verificare la modifica della collezione di righe e rimanere sincronizzato con essa. |

### Valore di ritorno

L'enumeratore di righe che attraverserà tutte le righe esistenti in questa collezione.

### Osservazioni

Se la collezione di righe verrà modificata (da operazioni che possono causare l'instanziazione di una nuova Row o la rimozione di una Row esistente) durante l'attraversamento con l'enumeratore, dovrebbe essere utilizzato l'enumeratore sincronizzato invece dell'enumeratore normale affinché l'attraversamento possa continuare dalla posizione subito dopo quella attraversata dall'ultimo MoveNext(). Tuttavia, insieme al vantaggio che nessun elemento venga saltato o attraversato più volte, lo svantaggio dell'enumeratore sincronizzato è che le prestazioni saranno leggermente degradate rispetto all'enumeratore normale.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Collections;

    public class RowCollectionMethodGetEnumeratorWithBooleanBooleanDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi alcuni dati di esempio alle righe
            for (int i = 0; i < 5; i++)
            {
                Row row = worksheet.Cells.Rows[i];
                row[0].PutValue($"Row {i + 1}");
            }
            
            try
            {
                // Ottieni la RowCollection
                RowCollection rows = worksheet.Cells.Rows;
                
                // Chiama GetEnumerator con i parametri (reversed: true, sync: false)
                IEnumerator enumerator = rows.GetEnumerator(true, false);
                
                Console.WriteLine("Iterating rows in reverse order:");
                while (enumerator.MoveNext())
                {
                    Row row = (Row)enumerator.Current;
                    Console.WriteLine(row[0].StringValue);
                }
                
                // Chiama GetEnumerator con i parametri (reversed: false, sync: true)
                enumerator = rows.GetEnumerator(false, true);
                
                Console.WriteLine("\nIterating rows in normal order (synchronized):");
                while (enumerator.MoveNext())
                {
                    Row row = (Row)enumerator.Current;
                    Console.WriteLine(row[0].StringValue);
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetEnumerator method: {ex.Message}");
            }
            
            // Salva il risultato
            workbook.Save("RowCollectionGetEnumeratorDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [RowCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



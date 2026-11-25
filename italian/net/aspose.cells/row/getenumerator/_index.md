---
title: "Row.GetEnumerator"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Row. Ottiene l'enumeratore delle celle"
type: docs
url: /it/net/aspose.cells/row/getenumerator/
---
## GetEnumerator() {#getenumerator}

Ottiene l'enumeratore delle celle

```csharp
public IEnumerator GetEnumerator()
```

### Valore di ritorno

L'enumeratore delle celle che attraverserà tutte le celle esistenti in questa riga.

### Esempi

```csharp
using System;
using System.Collections;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowMethodGetEnumeratorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Popola alcuni dati di esempio
            cells["A1"].PutValue("Name");
            cells["B1"].PutValue("Age");
            cells["A2"].PutValue("John");
            cells["B2"].PutValue(30);
            cells["A3"].PutValue("Alice");
            cells["B3"].PutValue(25);

            // Ottieni l'enumeratore per la prima riga (riga di intestazione)
            IEnumerator en = cells.Rows[0].GetEnumerator();
            while (en.MoveNext())
            {
                Cell cell = (Cell)en.Current;
                Console.WriteLine(cell.Name + ": " + cell.Value);
            }
        }
    }
}
```

### Vedi anche

* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetEnumerator(bool, bool) {#getenumerator_1}

Ottiene un enumeratore che itera le celle attraverso questa riga.

```csharp
public IEnumerator GetEnumerator(bool reversed, bool sync)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| invertito | Booleano | se enumerare le celle in ordine inverso |
| sync | Booleano | se l'enumeratore restituito dovrebbe controllare la modifica delle celle in questa riga e mantenerlo sincronizzato con essa. |

### Valore di ritorno

L'enumeratore delle celle che attraverserà tutte le celle esistenti in questa riga.

### Osservazioni

Se la riga verrà modificata (tramite operazioni che possono causare l'instanziazione di una nuova Cell o la rimozione di una Cell esistente) durante l'attraversamento con l'enumeratore, dovrebbe essere usato un enumeratore sincronizzato invece di un enumeratore normale affinché l'attraversamento possa continuare dalla posizione subito dopo quella attraversata dall'ultimo MoveNext(). Tuttavia, oltre al vantaggio che nessun elemento venga saltato o attraversato più volte, lo svantaggio dell'enumeratore sincronizzato è che le prestazioni saranno leggermente degradate rispetto a un enumeratore normale.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Collections;

    public class RowMethodGetEnumeratorWithBooleanBooleanDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi alcuni dati alle celle nella prima riga
            Row row = worksheet.Cells.Rows[0];
            worksheet.Cells["A1"].PutValue("Cell A1");
            worksheet.Cells["B1"].PutValue("Cell B1");
            worksheet.Cells["C1"].PutValue("Cell C1");

            try
            {
                // Chiama GetEnumerator con reversed=false e sync=true
                IEnumerator enumerator = row.GetEnumerator(false, true);
                
                Console.WriteLine("Cells in row 1:");
                while (enumerator.MoveNext())
                {
                    Cell cell = (Cell)enumerator.Current;
                    if (cell != null)
                    {
                        Console.WriteLine($"Cell {cell.Name}: {cell.Value}");
                    }
                }

                // Chiama GetEnumerator con reversed=true e sync=false per dimostrare l'iterazione inversa
                Console.WriteLine("\nCells in row 1 (reversed order):");
                enumerator = row.GetEnumerator(true, false);
                while (enumerator.MoveNext())
                {
                    Cell cell = (Cell)enumerator.Current;
                    if (cell != null)
                    {
                        Console.WriteLine($"Cell {cell.Name}: {cell.Value}");
                    }
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetEnumerator method: {ex.Message}");
            }

            // Salva la cartella di lavoro
            workbook.Save("RowMethodGetEnumeratorWithBooleanBooleanDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



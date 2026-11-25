---
title: "CellWatchCollection.Add"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "CellWatchCollection metodo. Aggiunge CellWatch con una riga e una colonna"
type: docs
url: /it/net/aspose.cells/cellwatchcollection/add/
---
## Add(int, int) {#add}

Aggiunge [`CellWatch`](../../cellwatch/) con una riga e una colonna.

```csharp
public int Add(int row, int column)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| riga | Int32 | L'indice della riga. |
| colonna | Int32 | L'indice della colonna. |

### Valore di ritorno

Restituisce la posizione di questo elemento nella raccolta.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellWatchCollectionMethodAddWithInt32Int32Demo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ottieni la CellWatchCollection dal foglio di lavoro
            CellWatchCollection cellWatchCollection = worksheet.CellWatches;
            
            try
            {
                // Chiama il metodo Add con gli indici di riga e colonna (Int32, Int32)
                int index = cellWatchCollection.Add(5, 3); // Adding cell at row 6, column D (0-based)
                
                Console.WriteLine($"CellWatch added at index: {index}");
                
                // Verifica il monitor della cella aggiunto
                CellWatch cellWatch = cellWatchCollection[index];
                Console.WriteLine($"Watching cell: {cellWatch.Row},{cellWatch.Column}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }
            
            // Salva il risultato
            workbook.Save("CellWatchCollectionMethodAddWithInt32Int32Demo.xlsx");
        }
    }
}
```

### Vedi anche

* class [CellWatchCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(string) {#add_1}

Aggiunge [`CellWatch`](../../cellwatch/) con il nome della cella.

```csharp
public int Add(string cellName)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| cellName | String | Il nome della cella. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellWatchCollectionMethodAddWithStringDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi alcuni monitor di celle
            worksheet.CellWatches.Add("A1");
            worksheet.CellWatches.Add("B2");
            worksheet.CellWatches.Add("C3");
            
            // Visualizza il conteggio dei monitor delle celle
            Console.WriteLine("Cell Watches Count: " + worksheet.CellWatches.Count);
            
            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [CellWatchCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



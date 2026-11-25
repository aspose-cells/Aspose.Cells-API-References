---
title: "HorizontalPageBreakCollection.Item"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà HorizontalPageBreakCollection. Ottiene l'elemento HorizontalPageBreak all'indice specificato"
type: docs
url: /it/net/aspose.cells/horizontalpagebreakcollection/item/
---
## HorizontalPageBreakCollection indexer (1 of 2)

Ottiene l'elemento [`HorizontalPageBreak`](../../horizontalpagebreak/) all'indice specificato.

```csharp
public HorizontalPageBreak this[int index] { get; }
```

| Parametro | Descrizione |
| --- | --- |
| indice | L'indice a base zero dell'elemento. |

### Valore di ritorno

L'elemento all'indice specificato.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HorizontalPageBreakCollectionPropertyItemDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi interruzioni di pagina orizzontali
            worksheet.HorizontalPageBreaks.Add(5);
            worksheet.HorizontalPageBreaks.Add(10);
            
            // Accedi alle interruzioni di pagina usando la proprietà Item
            HorizontalPageBreak firstBreak = worksheet.HorizontalPageBreaks[0];
            Console.WriteLine("First page break row: " + firstBreak.Row);
            
            // Modifica le celle che influiscono sulle interruzioni di pagina
            worksheet.Cells.DeleteRows(0, 2);
            
            // Verifica che l'interruzione di pagina sia stata regolata
            Console.WriteLine("First page break after row deletion: " + worksheet.HorizontalPageBreaks[0].Row);
        }
    }
}
```

### Vedi anche

* class [HorizontalPageBreak](../../horizontalpagebreak/)
* class [HorizontalPageBreakCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## HorizontalPageBreakCollection indexer (2 of 2)

Ottiene l'elemento [`HorizontalPageBreak`](../../horizontalpagebreak/) con il nome della cella specificato.

```csharp
public HorizontalPageBreak this[string cellName] { get; }
```

| Parametro | Descrizione |
| --- | --- |
| cellName | Nome della cella. |

### Valore di ritorno

L'elemento con il nome cella specificato.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using System;
    using Aspose.Cells;

    public class HorizontalPageBreakCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            // Crea una nuova cartella di lavoro e ottieni il primo foglio di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Aggiungi un paio di interruzioni di pagina orizzontali usando overload diversi
                worksheet.HorizontalPageBreaks.Add(5);          // break after row index 5
                worksheet.HorizontalPageBreaks.Add("D5");      // break at cell D5 (row index 4)

                // ----- Accesso tramite indice intero (Item[int]) -----
                // La proprietà Item è l'indicizzatore, quindi usiamo la sintassi []
                HorizontalPageBreak firstBreak = worksheet.HorizontalPageBreaks[0];
                Console.WriteLine("First break row (int index): " + firstBreak.Row);

                // ----- Accesso tramite chiave stringa (Item[string]) -----
                // Recupera l'interruzione di pagina aggiunta con il nome della cella "D5"
                HorizontalPageBreak breakByCell = worksheet.HorizontalPageBreaks["D5"];
                Console.WriteLine("Break added with \"D5\" is at row: " + breakByCell.Row);

                // Salva la cartella di lavoro per verificare che le interruzioni di pagina siano persistenti
                workbook.Save("HorizontalPageBreaks_ItemDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine("Error: " + ex.Message);
            }
        }
    }
}
```

### Vedi anche

* class [HorizontalPageBreak](../../horizontalpagebreak/)
* class [HorizontalPageBreakCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



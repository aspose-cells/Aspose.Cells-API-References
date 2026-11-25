---
title: "VerticalPageBreakCollection.Item"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà VerticalPageBreakCollection. Ottiene l'elemento VerticalPageBreak all'indice specificato"
type: docs
url: /it/net/aspose.cells/verticalpagebreakcollection/item/
---
## VerticalPageBreakCollection indexer (1 of 2)

Ottiene l'elemento [`VerticalPageBreak`](../../verticalpagebreak/) all'indice specificato.

```csharp
public VerticalPageBreak this[int index] { get; }
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
    public class VerticalPageBreakCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi interruzioni di pagina verticali
            worksheet.VerticalPageBreaks.Add(5);
            worksheet.VerticalPageBreaks.Add(10);
            worksheet.VerticalPageBreaks.Add(15);

            // Accedi e visualizza le interruzioni di pagina usando la proprietà Item
            VerticalPageBreakCollection vpagebreaks = worksheet.VerticalPageBreaks;
            Console.WriteLine("Vertical Page Breaks:");
            for (int i = 0; i < vpagebreaks.Count; i++)
            {
                Console.WriteLine($"Break {i + 1}: Column = {vpagebreaks[i].Column}");
            }

            // Rimuovere e riaggiungere per modificare un'interruzione di pagina poiché Column è di sola lettura
            int column = vpagebreaks[1].Column;
            vpagebreaks.RemoveAt(1);
            vpagebreaks.Add(12);
            Console.WriteLine("\nAfter modification:");
            Console.WriteLine($"Break 2: Column = {vpagebreaks[1].Column}");
        }
    }
}
```

### Vedi anche

* class [VerticalPageBreak](../../verticalpagebreak/)
* class [VerticalPageBreakCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## VerticalPageBreakCollection indexer (2 of 2)

Ottiene l'elemento [`VerticalPageBreak`](../../verticalpagebreak/) con il nome cella specificato.

```csharp
public VerticalPageBreak this[string cellName] { get; }
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
    using Aspose.Cells;
    using System;

    public class VerticalPageBreakCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi alcune interruzioni di pagina verticali
            worksheet.VerticalPageBreaks.Add(3);
            worksheet.VerticalPageBreaks.Add(7);

            try
            {
                // Accedi a VerticalPageBreakCollection
                VerticalPageBreakCollection pageBreaks = worksheet.VerticalPageBreaks;

                // Dimostra l'accesso agli elementi usando la proprietà Item (indicizzatore)
                Console.WriteLine("Vertical Page Breaks in the worksheet:");
                for (int i = 0; i < pageBreaks.Count; i++)
                {
                    VerticalPageBreak vpb = pageBreaks[i];
                    Console.WriteLine($"Break {i + 1}: Column = {vpb.Column}, StartRow = {vpb.StartRow}, EndRow = {vpb.EndRow}");
                }

                // Salva la cartella di lavoro
                workbook.Save("VerticalPageBreakItemDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [VerticalPageBreak](../../verticalpagebreak/)
* class [VerticalPageBreakCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



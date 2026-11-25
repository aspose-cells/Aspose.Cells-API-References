---
title: "Classe HorizontalPageBreak"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.HorizontalPageBreak classe. Incapsula l'oggetto che rappresenta un'interruzione di pagina orizzontale"
type: docs
url: /it/net/aspose.cells/horizontalpagebreak/
---
## HorizontalPageBreak class

Incapsula l'oggetto che rappresenta un'interruzione di pagina orizzontale.

```csharp
public class HorizontalPageBreak
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [EndColumn](../../aspose.cells/horizontalpagebreak/endcolumn/) { get; } | Restituisce l'indice della colonna finale di questa interruzione di pagina orizzontale. |
| [Row](../../aspose.cells/horizontalpagebreak/row/) { get; } | Restituisce l'indice della riga basato su zero. |
| [StartColumn](../../aspose.cells/horizontalpagebreak/startcolumn/) { get; } | Restituisce l'indice della colonna iniziale di questa interruzione di pagina orizzontale. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class HorizontalPageBreakDemo
    {
        public static void HorizontalPageBreakExample()
        {
            // Istanziare un oggetto Workbook
            Workbook workbook = new Workbook();
            
            // Ottenere il riferimento del foglio di lavoro appena aggiunto passando il suo indice di foglio
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi un'interruzione di pagina nella cella Y30
            int index = worksheet.HorizontalPageBreaks.Add("Y30");
            
            // Ottieni l'interruzione di pagina orizzontale appena aggiunta
            HorizontalPageBreak hPageBreak = worksheet.HorizontalPageBreaks[index];
            
            // Visualizza le proprietà dell'interruzione di pagina orizzontale
            Console.WriteLine("Horizontal Page Break Details:");
            Console.WriteLine($"Row: {hPageBreak.Row}");
            Console.WriteLine($"Start Column: {hPageBreak.StartColumn}");
            Console.WriteLine($"End Column: {hPageBreak.EndColumn}");
            
            // Salva la cartella di lavoro
            workbook.Save("HorizontalPageBreakExample.xlsx");
            workbook.Save("HorizontalPageBreakExample.pdf");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)



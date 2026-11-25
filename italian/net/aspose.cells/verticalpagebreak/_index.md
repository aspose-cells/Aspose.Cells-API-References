---
title: "Classe VerticalPageBreak"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.VerticalPageBreak. Incapsula l'oggetto che rappresenta un'interruzione di pagina verticale"
type: docs
url: /it/net/aspose.cells/verticalpagebreak/
---
## VerticalPageBreak class

Incapsula l'oggetto che rappresenta un'interruzione di pagina verticale.

```csharp
public class VerticalPageBreak
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Column](../../aspose.cells/verticalpagebreak/column/) { get; } | Restituisce l'indice della colonna dell'interruzione di pagina verticale. |
| [EndRow](../../aspose.cells/verticalpagebreak/endrow/) { get; } | Restituisce l'indice della riga finale dell'interruzione di pagina verticale. |
| [StartRow](../../aspose.cells/verticalpagebreak/startrow/) { get; } | Restituisce l'indice della riga iniziale dell'interruzione di pagina verticale. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class VerticalPageBreakDemo
    {
        public static void VerticalPageBreakExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro nella cartella di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi un'interruzione di pagina verticale nella colonna G (indice 6)
            worksheet.VerticalPageBreaks.Add("G5");

            // Salva la cartella di lavoro
            workbook.Save("VerticalPageBreakExample.xlsx");

            // Accedi all'interruzione di pagina verticale aggiunta
            VerticalPageBreak vpb = worksheet.VerticalPageBreaks[0];

            // Visualizza le proprietà dell'interruzione di pagina verticale
            Console.WriteLine("Start Row: " + vpb.StartRow);
            Console.WriteLine("End Row: " + vpb.EndRow);
            Console.WriteLine("Column: " + vpb.Column);
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)



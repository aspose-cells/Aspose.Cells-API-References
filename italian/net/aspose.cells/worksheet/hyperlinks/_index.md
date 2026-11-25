---
title: "Worksheet.Hyperlinks"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Worksheet. Ottiene la collezione HyperlinkCollection"
type: docs
url: /it/net/aspose.cells/worksheet/hyperlinks/
---
## Worksheet.Hyperlinks property

Ottiene la collezione [`HyperlinkCollection`](../../hyperlinkcollection/).

```csharp
public HyperlinkCollection Hyperlinks { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyHyperlinksDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi un collegamento ipertestuale al foglio di lavoro
            worksheet.Hyperlinks.Add(0, 0, 1, 1, @"https://www.aspose.com");
            
            // Salva la cartella di lavoro
            workbook.Save("HyperlinksDemo.xlsx");
            
            // Carica la cartella di lavoro salvata per verificare il collegamento ipertestuale
            Workbook loadedWorkbook = new Workbook("HyperlinksDemo.xlsx");
            Worksheet loadedWorksheet = loadedWorkbook.Worksheets[0];
            
            // Visualizza l'indirizzo del collegamento ipertestuale.
            Console.WriteLine("Hyperlink Address: " + loadedWorksheet.Hyperlinks[0].Address);
        }
    }
}
```

### Vedi anche

* class [HyperlinkCollection](../../hyperlinkcollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



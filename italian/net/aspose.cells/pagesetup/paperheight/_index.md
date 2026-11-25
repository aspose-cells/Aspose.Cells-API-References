---
title: "PageSetup.PaperHeight"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PageSetup. Ottiene l'altezza della carta in unità di pollici, considerata l'orientamento della pagina"
type: docs
url: /it/net/aspose.cells/pagesetup/paperheight/
---
## PageSetup.PaperHeight property

Ottiene l'altezza della carta in unità di pollici, considerata l'orientazione della pagina.

```csharp
public double PaperHeight { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyPaperHeightDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Imposta alcuni dati in una cella
            worksheet.Cells["A1"].PutValue("Paper Height Demo");
            
            // Ottieni l'oggetto PageSetup
            PageSetup pageSetup = worksheet.PageSetup;
            
            // Visualizza l'altezza predefinita della carta (in pollici)
            Console.WriteLine("Default Paper Height: " + pageSetup.PaperHeight);
            
            // PaperHeight è di sola lettura, quindi dimostriamo come ottenere diverse dimensioni della carta
            // cambiando il tipo di formato della carta a Letter (8,5x11 pollici)
            pageSetup.PaperSize = PaperSizeType.PaperLetter;
            
            // Verifica la modifica
            Console.WriteLine("Modified Paper Height (Letter size): " + pageSetup.PaperHeight);
        }
    }
}
```

### Vedi anche

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



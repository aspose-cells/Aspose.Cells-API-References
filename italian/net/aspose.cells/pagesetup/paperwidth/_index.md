---
title: "PageSetup.PaperWidth"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PageSetup. Ottiene la larghezza della carta nell'unità di pollici considerata l'orientamento della pagina"
type: docs
url: /it/net/aspose.cells/pagesetup/paperwidth/
---
## PageSetup.PaperWidth property

Ottiene la larghezza della carta in unità di pollici, considerata l'orientazione della pagina.

```csharp
public double PaperWidth { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyPaperWidthDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Imposta alcuni dati di esempio
            worksheet.Cells["A1"].PutValue("Sample Page Setup Demo");
            
            // Accedi al PageSetup del foglio di lavoro
            PageSetup pageSetup = worksheet.PageSetup;
            
            // Dimostra la proprietà PaperWidth (sola lettura)
            Console.WriteLine("Paper Width: " + pageSetup.PaperWidth);
            
            // Per modificare le dimensioni della carta, usa invece la proprietà PaperSize
            pageSetup.PaperSize = PaperSizeType.PaperLetter;
            Console.WriteLine("New Paper Width: " + pageSetup.PaperWidth);
        }
    }
}
```

### Vedi anche

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



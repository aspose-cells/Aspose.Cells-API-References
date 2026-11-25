---
title: "PageSetup.IsAutomaticPaperSize"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PageSetup. Indica se la dimensione della carta è automatica"
type: docs
url: /it/net/aspose.cells/pagesetup/isautomaticpapersize/
---
## PageSetup.IsAutomaticPaperSize property

Indica se la dimensione della carta è automatica.

```csharp
public bool IsAutomaticPaperSize { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyIsAutomaticPaperSizeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Accedi alla configurazione della pagina
            PageSetup pageSetup = worksheet.PageSetup;
            
            // Ottieni il valore della dimensione della carta automatica
            Console.WriteLine("Automatic Paper Size: " + pageSetup.IsAutomaticPaperSize);
            
            // Crea un'altra cartella di lavoro con impostazioni diverse
            Workbook workbook2 = new Workbook("example.xlsx");
            PageSetup pageSetup2 = workbook2.Worksheets[0].PageSetup;
            Console.WriteLine("Automatic Paper Size from file: " + pageSetup2.IsAutomaticPaperSize);
        }
    }
}
```

### Vedi anche

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



---
title: "PageSetup.FitToPagesWide"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PageSetup. Rappresenta il numero di pagine in larghezza a cui il foglio di lavoro sarà scalato quando stampato. Il valore predefinito è 1"
type: docs
url: /it/net/aspose.cells/pagesetup/fittopageswide/
---
## PageSetup.FitToPagesWide property

Rappresenta il numero di pagine in larghezza a cui il foglio di lavoro verrà scalato quando viene stampato. Il valore predefinito è 1.

```csharp
public int FitToPagesWide { get; set; }
```

### Osservazioni

Devi impostare FitToPagesTall a zero se vuoi adattare tutte le colonne su una pagina.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyFitToPagesWideDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio alle celle
            worksheet.Cells["A1"].PutValue("Sample Data 1");
            worksheet.Cells["A2"].PutValue("Sample Data 2");
            worksheet.Cells["B1"].PutValue("Sample Data 3");
            worksheet.Cells["B2"].PutValue("Sample Data 4");

            // Imposta le proprietà di configurazione della pagina
            worksheet.PageSetup.FitToPagesWide = 1;  // Fit to 1 page wide
            worksheet.PageSetup.FitToPagesTall = 0; // Let height adjust automatically

            // Salva la cartella di lavoro
            workbook.Save("FitToPagesWideDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



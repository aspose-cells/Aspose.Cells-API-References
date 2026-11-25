---
title: "PageSetup.PrintQuality"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PageSetup. Rappresenta la qualità di stampa"
type: docs
url: /it/net/aspose.cells/pagesetup/printquality/
---
## PageSetup.PrintQuality property

Rappresenta la qualità di stampa.

```csharp
public int PrintQuality { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyPrintQualityDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Imposta la qualità di stampa a 144 dpi
            worksheet.PageSetup.PrintQuality = 144;
            
            // Stampa l'impostazione corrente della qualità di stampa
            Console.WriteLine("Print Quality: " + worksheet.PageSetup.PrintQuality);
            
            // Salva la cartella di lavoro
            workbook.Save("PrintQualityDemo.xls");
        }
    }
}
```

### Vedi anche

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



---
title: "PageSetup.Zoom"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PageSetup. Rappresenta il fattore di scala in percentuale. Deve essere compreso tra 10 e 400"
type: docs
url: /it/net/aspose.cells/pagesetup/zoom/
---
## PageSetup.Zoom property

Rappresenta il fattore di scala in percentuale. Deve essere compreso tra 10 e 400.

```csharp
public int Zoom { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyZoomDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Imposta il livello di zoom al 150%
            worksheet.PageSetup.Zoom = 150;
            
            // Stampa il livello di zoom corrente
            Console.WriteLine("Current Zoom Level: " + worksheet.PageSetup.Zoom);
            
            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



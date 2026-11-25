---
title: "PageSetup.BlackAndWhite"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PageSetup. Rappresenta se gli elementi del documento verranno stampati in bianco e nero"
type: docs
url: /it/net/aspose.cells/pagesetup/blackandwhite/
---
## PageSetup.BlackAndWhite property

Rappresenta se gli elementi del documento verranno stampati in bianco e nero.

```csharp
public bool BlackAndWhite { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyBlackAndWhiteDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ottieni l'oggetto PageSetup
            PageSetup pageSetup = worksheet.PageSetup;

            // Imposta la proprietà BlackAndWhite su true
            pageSetup.BlackAndWhite = true;
            Console.WriteLine("BlackAndWhite set to: " + pageSetup.BlackAndWhite);

            // Modifica la proprietà BlackAndWhite su false
            pageSetup.BlackAndWhite = false;
            Console.WriteLine("BlackAndWhite changed to: " + pageSetup.BlackAndWhite);

            // Salva la cartella di lavoro
            workbook.Save("PageSetupBlackAndWhiteDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



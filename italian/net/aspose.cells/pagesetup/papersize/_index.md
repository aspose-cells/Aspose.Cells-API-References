---
title: "PageSetup.PaperSize"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PageSetup. Rappresenta la dimensione della carta"
type: docs
url: /it/net/aspose.cells/pagesetup/papersize/
---
## PageSetup.PaperSize property

Rappresenta la dimensione della carta.

```csharp
public PaperSizeType PaperSize { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyPaperSizeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Imposta la dimensione della carta su Envelope B6
            sheet.PageSetup.PaperSize = PaperSizeType.PaperEnvelopeB6;

            // Stampa la dimensione della carta corrente
            Console.WriteLine("Current paper size: " + sheet.PageSetup.PaperSize);

            // Salva la cartella di lavoro
            workbook.Save("PageSetup_PaperSizeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [PaperSizeType](../../papersizetype/)
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



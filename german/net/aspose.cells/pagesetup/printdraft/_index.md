---
title: "PageSetup.PrintDraft"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PageSetup-Eigenschaft. Gibt an, ob das Blatt ohne Grafiken gedruckt wird"
type: docs
url: /de/net/aspose.cells/pagesetup/printdraft/
---
## PageSetup.PrintDraft property

Stellt dar, ob das Blatt ohne Grafiken gedruckt wird.

```csharp
public bool PrintDraft { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyPrintDraftDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Greifen Sie auf das PageSetup-Objekt zu
            PageSetup pageSetup = worksheet.PageSetup;

            // Setze die PrintDraft-Eigenschaft auf true
            pageSetup.PrintDraft = true;
            Console.WriteLine("PrintDraft set to: " + pageSetup.PrintDraft);

            // Ändere die PrintDraft-Eigenschaft auf false
            pageSetup.PrintDraft = false;
            Console.WriteLine("PrintDraft changed to: " + pageSetup.PrintDraft);

            // Speichere die Arbeitsmappe
            workbook.Save("PageSetup_PrintDraft_Example.xlsx");
        }
    }
}
```

### Siehe auch

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



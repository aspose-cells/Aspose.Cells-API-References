---
title: "PageSetup.IsHFDiffFirst"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PageSetup-Eigenschaft. True bedeutet, dass die Kopf-/Fußzeile der ersten Seite sich von den anderen Seiten unterscheidet"
type: docs
url: /de/net/aspose.cells/pagesetup/ishfdifffirst/
---
## PageSetup.IsHFDiffFirst property

Wahr bedeutet, dass die Kopf-/Fußzeile der ersten Seite sich von den anderen Seiten unterscheidet.

```csharp
public bool IsHFDiffFirst { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyIsHFDiffFirstDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Zugriff auf PageSetup
            PageSetup pageSetup = worksheet.PageSetup;
            
            // Unterschiedliche Kopf‑/Fußzeilen für die erste Seite festlegen
            pageSetup.IsHFDiffFirst = true;
            
            // Kopf‑/Fußzeilen festlegen
            pageSetup.SetFirstPageHeader(0, "First Page Header");
            pageSetup.SetHeader(0, "Standard Header");
            
            // Speichere die Arbeitsmappe
            workbook.Save("PageSetup_IsHFDiffFirst_Example.xlsx");
            
            // Arbeitsmappe neu laden, um die Einstellungen zu überprüfen
            Workbook loadedWorkbook = new Workbook("PageSetup_IsHFDiffFirst_Example.xlsx");
            PageSetup loadedPageSetup = loadedWorkbook.Worksheets[0].PageSetup;
            
            // Ausgabeüberprüfung
            Console.WriteLine("IsHFDiffFirst: " + loadedPageSetup.IsHFDiffFirst);
            Console.WriteLine("First Page Header: " + loadedPageSetup.GetFirstPageHeader(0));
            Console.WriteLine("Standard Header: " + loadedPageSetup.GetHeader(0));
        }
    }
}
```

### Siehe auch

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



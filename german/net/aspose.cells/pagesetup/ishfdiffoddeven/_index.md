---
title: "PageSetup.IsHFDiffOddEven"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PageSetup-Eigenschaft. True bedeutet, dass die Kopf‑/Fußzeile der ungeraden Seiten von der der geraden Seiten abweicht"
type: docs
url: /de/net/aspose.cells/pagesetup/ishfdiffoddeven/
---
## PageSetup.IsHFDiffOddEven property

Wahr bedeutet, dass die Kopf-/Fußzeile der ungeraden Seiten sich von den ungeraden Seiten unterscheidet.

```csharp
public bool IsHFDiffOddEven { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyIsHFDiffOddEvenDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Zugriff auf PageSetup
            PageSetup pageSetup = worksheet.PageSetup;
            
            // Aktiviere unterschiedliche Kopf‑/Fußzeilen für ungerade und gerade Seiten
            pageSetup.IsHFDiffOddEven = true;
            
            // Unterschiedliche Fußzeilen für ungerade und gerade Seiten festlegen
            pageSetup.SetFooter(0, "Odd Page Footer");
            pageSetup.SetEvenFooter(0, "Even Page Footer");
            
            // Speichere die Arbeitsmappe
            workbook.Save("PageSetup_IsHFDiffOddEven_Example.xlsx");
            
            // Überprüfen Sie die Einstellungen, indem Sie die gespeicherte Datei laden
            Workbook loadedWorkbook = new Workbook("PageSetup_IsHFDiffOddEven_Example.xlsx");
            PageSetup loadedPageSetup = loadedWorkbook.Worksheets[0].PageSetup;
            
            Console.WriteLine("IsHFDiffOddEven: " + loadedPageSetup.IsHFDiffOddEven);
            Console.WriteLine("Odd Page Footer: " + loadedPageSetup.GetFooter(0));
            Console.WriteLine("Even Page Footer: " + loadedPageSetup.GetEvenFooter(0));
        }
    }
}
```

### Siehe auch

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



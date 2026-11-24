---
title: "PageSetup.PrintCopies"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PageSetup‑Eigenschaft. Gibt die Anzahl der zu druckenden Kopien zurück und legt sie fest"
type: docs
url: /de/net/aspose.cells/pagesetup/printcopies/
---
## PageSetup.PrintCopies property

Liest und setzt die Anzahl der zu druckenden Kopien.

```csharp
public int PrintCopies { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyPrintCopiesDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Setze die Anzahl der Druckkopien auf 3
            worksheet.PageSetup.PrintCopies = 3;
            
            // Zeige die aktuelle Einstellung der Druckkopien an
            Console.WriteLine("Print Copies: " + worksheet.PageSetup.PrintCopies);
            
            // Speichere die Arbeitsmappe
            workbook.Save("PageSetup_PrintCopies_Output.xlsx");
        }
    }
}
```

### Siehe auch

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



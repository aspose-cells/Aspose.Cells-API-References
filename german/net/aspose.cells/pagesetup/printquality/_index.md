---
title: "PageSetup.PrintQuality"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PageSetup-Eigenschaft. Gibt die Druckqualität an."
type: docs
url: /de/net/aspose.cells/pagesetup/printquality/
---
## PageSetup.PrintQuality property

Stellt die Druckqualität dar.

```csharp
public int PrintQuality { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyPrintQualityDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Stellen Sie die Druckqualität auf 144 dpi ein.
            worksheet.PageSetup.PrintQuality = 144;
            
            // Geben Sie die aktuelle Druckqualitätseinstellung aus.
            Console.WriteLine("Print Quality: " + worksheet.PageSetup.PrintQuality);
            
            // Speichere die Arbeitsmappe
            workbook.Save("PrintQualityDemo.xls");
        }
    }
}
```

### Siehe auch

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



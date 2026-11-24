---
title: "PageSetup.PrintTitleRows"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PageSetup-Eigenschaft. Stellt die Zeilen dar, die die Zellen enthalten, die oben auf jeder Seite wiederholt werden."
type: docs
url: /de/net/aspose.cells/pagesetup/printtitlerows/
---
## PageSetup.PrintTitleRows property

Stellt die Zeilen dar, die die Zellen enthalten, die oben auf jeder Seite wiederholt werden.

```csharp
public string PrintTitleRows { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyPrintTitleRowsDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Beispieldaten festlegen
            worksheet.Cells["A1"].PutValue("Header");
            for (int i = 2; i <= 10; i++)
            {
                worksheet.Cells["A" + i].PutValue("Data " + (i-1));
            }
            
            // Greife auf die Seiteneinrichtung zu
            PageSetup pageSetup = worksheet.PageSetup;
            
            // Drucktitelzeilen festlegen (erste Zeile wird auf jeder gedruckten Seite wiederholt)
            pageSetup.PrintTitleRows = "$1:$1";
            
            // Speichere die Arbeitsmappe
            workbook.Save("PrintTitleRowsDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



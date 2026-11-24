---
title: "PageSetup.PrintGridlines"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PageSetup-Eigenschaft. Gibt an, ob Zellgitternetzlinien auf der Seite gedruckt werden."
type: docs
url: /de/net/aspose.cells/pagesetup/printgridlines/
---
## PageSetup.PrintGridlines property

Stellt dar, ob Zellenrasterlinien auf der Seite gedruckt werden.

```csharp
public bool PrintGridlines { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyPrintGridlinesDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fügen Sie Beispieldaten in die Zelle ein.
            worksheet.Cells["A1"].PutValue("PrintGridlines Property Demo");
            worksheet.Cells["A3"].PutValue("Gridlines will ");
            worksheet.Cells["B3"].PutValue(worksheet.PageSetup.PrintGridlines ? "appear" : "not appear");
            worksheet.Cells["A4"].PutValue("when printing this sheet.");

            // Schalten Sie die PrintGridlines-Eigenschaft um.
            worksheet.PageSetup.PrintGridlines = true;
            
            // Speichere die Arbeitsmappe
            workbook.Save("PrintGridlinesDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



---
title: "PageSetup.FitToPagesWide"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PageSetup-Eigenschaft. Gibt die Anzahl der Seiten in der Breite an, auf die das Arbeitsblatt beim Drucken skaliert wird. Der Standardwert ist 1."
type: docs
url: /de/net/aspose.cells/pagesetup/fittopageswide/
---
## PageSetup.FitToPagesWide property

Gibt die Anzahl der Seiten in der Breite an, auf die das Arbeitsblatt beim Drucken skaliert wird. Der Standardwert ist 1.

```csharp
public int FitToPagesWide { get; set; }
```

### Hinweise

Sie müssen FitToPagesTall auf null setzen, wenn Sie alle Spalten auf einer Seite anpassen möchten.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyFitToPagesWideDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge Beispieldaten zu Zellen hinzu
            worksheet.Cells["A1"].PutValue("Sample Data 1");
            worksheet.Cells["A2"].PutValue("Sample Data 2");
            worksheet.Cells["B1"].PutValue("Sample Data 3");
            worksheet.Cells["B2"].PutValue("Sample Data 4");

            // Seitenlayout-Eigenschaften festlegen
            worksheet.PageSetup.FitToPagesWide = 1;  // Fit to 1 page wide
            worksheet.PageSetup.FitToPagesTall = 0; // Let height adjust automatically

            // Speichere die Arbeitsmappe
            workbook.Save("FitToPagesWideDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



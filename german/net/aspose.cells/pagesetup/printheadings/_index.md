---
title: "PageSetup.PrintHeadings"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PageSetup-Eigenschaft. Gibt an, ob Zeilen‑ und Spaltenüberschriften mit dieser Seite gedruckt werden."
type: docs
url: /de/net/aspose.cells/pagesetup/printheadings/
---
## PageSetup.PrintHeadings property

Stellt dar, ob Zeilen- und Spaltenüberschriften mit dieser Seite gedruckt werden.

```csharp
public bool PrintHeadings { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyPrintHeadingsDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Einige Beispieldaten mit Überschriften festlegen
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(2.5);
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B3"].PutValue(1.8);

            // Drucken von Überschriften aktivieren
            worksheet.PageSetup.PrintHeadings = true;
            worksheet.PageSetup.PrintArea = "A1:B3";

            // Als HTML speichern, um die Wirkung zu demonstrieren
            HtmlSaveOptions saveOptions = new HtmlSaveOptions
            {
                ExportActiveWorksheetOnly = true,
                ExportPrintAreaOnly = true,
                ExportGridLines = true,
                ExportHeadings = true
            };

            workbook.Save("PrintHeadingsDemo.html", saveOptions);

            Console.WriteLine("Worksheet saved with PrintHeadings enabled.");
        }
    }
}
```

### Siehe auch

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



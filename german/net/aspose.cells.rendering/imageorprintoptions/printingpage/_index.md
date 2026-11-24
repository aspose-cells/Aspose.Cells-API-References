---
title: "ImageOrPrintOptions.PrintingPage"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ImageOrPrintOptions-Eigenschaft. Gibt an, welche Seiten nicht gedruckt werden"
type: docs
url: /de/net/aspose.cells.rendering/imageorprintoptions/printingpage/
---
## ImageOrPrintOptions.PrintingPage property

Gibt an, welche Seiten nicht gedruckt werden.

```csharp
public PrintingPageType PrintingPage { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsPropertyPrintingPageDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Füge dem Arbeitsblatt einige Daten hinzu
            worksheet.Cells["A1"].PutValue("Test Data");
            worksheet.Cells["A2"].PutValue("Non-Blank Cell");
            worksheet.Cells["A5"].PutValue("Another Non-Blank Cell");
            
            // Bild-/Druckoptionen erstellen
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.PrintingPage = PrintingPageType.IgnoreBlank;
            
            // Rendern Sie die Arbeitsmappe mit den Optionen
            WorkbookRender render = new WorkbookRender(workbook, options);
            
            // Geben Sie die Seitenanzahl aus (leere Seiten werden ignoriert)
            Console.WriteLine("Page count with IgnoreBlank: " + render.PageCount);
            
            // Ändern Sie das Standardverhalten (alle Seiten einschließen)
            options.PrintingPage = PrintingPageType.Default;
            render = new WorkbookRender(workbook, options);
            Console.WriteLine("Page count with Default: " + render.PageCount);
        }
    }
}
```

### Siehe auch

* enum [PrintingPageType](../../../aspose.cells/printingpagetype/)
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)



---
title: "ImageOrPrintOptions.PrintingPage"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ImageOrPrintOptions-egenskap. Anger vilka sidor som inte kommer att skrivas ut"
type: docs
url: /sv/net/aspose.cells.rendering/imageorprintoptions/printingpage/
---
## ImageOrPrintOptions.PrintingPage property

Anger vilka sidor som inte kommer att skrivas ut.

```csharp
public PrintingPageType PrintingPage { get; set; }
```

### Exempel

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
            // Skapa en arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till lite data i kalkylbladet
            worksheet.Cells["A1"].PutValue("Test Data");
            worksheet.Cells["A2"].PutValue("Non-Blank Cell");
            worksheet.Cells["A5"].PutValue("Another Non-Blank Cell");
            
            // Skapa bild-/utskriftsalternativ
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.PrintingPage = PrintingPageType.IgnoreBlank;
            
            // Rendera arbetsboken med alternativen
            WorkbookRender render = new WorkbookRender(workbook, options);
            
            // Skriv ut sidantalet (kommer att ignorera tomma sidor)
            Console.WriteLine("Page count with IgnoreBlank: " + render.PageCount);
            
            // Ändra till standardbeteende (inkludera alla sidor)
            options.PrintingPage = PrintingPageType.Default;
            render = new WorkbookRender(workbook, options);
            Console.WriteLine("Page count with Default: " + render.PageCount);
        }
    }
}
```

### Se även

* enum [PrintingPageType](../../../aspose.cells/printingpagetype/)
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)



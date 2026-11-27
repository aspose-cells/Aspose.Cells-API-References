---
title: "SheetRender.PageCount"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SheetRender egenskap. Hämtar det totala sidantalet för det aktuella kalkylbladet"
type: docs
url: /sv/net/aspose.cells.rendering/sheetrender/pagecount/
---
## SheetRender.PageCount property

Hämtar det totala sidantalet för aktuellt kalkylblad.

```csharp
public int PageCount { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class SheetRenderPropertyPageCountDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata i kalkylbladet
            Cells cells = worksheet.Cells;
            cells["A1"].PutValue("Name");
            cells["B1"].PutValue("Age");
            cells["A2"].PutValue("John");
            cells["B2"].PutValue(30);
            cells["A3"].PutValue("Mary");
            cells["B3"].PutValue(25);
            cells["A4"].PutValue("Peter");
            cells["B4"].PutValue(35);

            // Ställ in sidinställning för utskrift
            PageSetup pageSetup = worksheet.PageSetup;
            pageSetup.PrintArea = "A1:B4";
            pageSetup.FitToPagesTall = 1;
            pageSetup.FitToPagesWide = 1;

            // Skapa SheetRender med standardalternativ
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            SheetRender render = new SheetRender(worksheet, options);

            // Visa sidantalet
            Console.WriteLine("Page Count: " + render.PageCount);

            // Ändra sidinställning för att tvinga flera sidor
            pageSetup.FitToPagesTall = 0;
            pageSetup.FitToPagesWide = 1;
            pageSetup.PrintArea = "A1:B100"; // Larger area than can fit on one page

            // Skapa ny SheetRender för att få uppdaterat sidantal
            SheetRender newRender = new SheetRender(worksheet, options);
            Console.WriteLine("Updated Page Count: " + newRender.PageCount);
        }
    }
}
```

### Se även

* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)



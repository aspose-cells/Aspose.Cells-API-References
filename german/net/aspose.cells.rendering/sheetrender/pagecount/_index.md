---
title: "SheetRender.PageCount"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SheetRender-Eigenschaft. Gibt die Gesamtseitenzahl des aktuellen Arbeitsblatts zurück"
type: docs
url: /de/net/aspose.cells.rendering/sheetrender/pagecount/
---
## SheetRender.PageCount property

Gibt die Gesamtseitenzahl des aktuellen Arbeitsblatts zurück.

```csharp
public int PageCount { get; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten zum Arbeitsblatt hinzufügen
            Cells cells = worksheet.Cells;
            cells["A1"].PutValue("Name");
            cells["B1"].PutValue("Age");
            cells["A2"].PutValue("John");
            cells["B2"].PutValue(30);
            cells["A3"].PutValue("Mary");
            cells["B3"].PutValue(25);
            cells["A4"].PutValue("Peter");
            cells["B4"].PutValue(35);

            // Seitenlayout für den Druck festlegen
            PageSetup pageSetup = worksheet.PageSetup;
            pageSetup.PrintArea = "A1:B4";
            pageSetup.FitToPagesTall = 1;
            pageSetup.FitToPagesWide = 1;

            // SheetRender mit Standardoptionen erstellen
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            SheetRender render = new SheetRender(worksheet, options);

            // Die Seitenzahl anzeigen
            Console.WriteLine("Page Count: " + render.PageCount);

            // Seitenlayout ändern, um mehrere Seiten zu erzwingen
            pageSetup.FitToPagesTall = 0;
            pageSetup.FitToPagesWide = 1;
            pageSetup.PrintArea = "A1:B100"; // Larger area than can fit on one page

            // Neues SheetRender erstellen, um die aktualisierte Seitenzahl zu erhalten
            SheetRender newRender = new SheetRender(worksheet, options);
            Console.WriteLine("Updated Page Count: " + newRender.PageCount);
        }
    }
}
```

### Siehe auch

* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)



---
title: "PageSetup.FitToPagesTall"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PageSetup-Eigenschaft. Gibt die Anzahl der Seiten in der Höhe an, auf die das Arbeitsblatt beim Drucken skaliert wird. Der Standardwert ist 1."
type: docs
url: /de/net/aspose.cells/pagesetup/fittopagestall/
---
## PageSetup.FitToPagesTall property

Gibt die Anzahl der Seiten in der Höhe an, auf die das Arbeitsblatt beim Drucken skaliert wird. Der Standardwert ist 1.

```csharp
public int FitToPagesTall { get; set; }
```

### Hinweise

Sie müssen FitToPagesWide auf Null setzen, wenn Sie alle Zeilen auf einer Seite unterbringen möchten.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyFitToPagesTallDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fügen Sie Beispieldaten hinzu, damit das Blatt über mehrere Seiten verteilt wird.
            for (int i = 0; i < 100; i++)
            {
                for (int j = 0; j < 10; j++)
                {
                    worksheet.Cells[i, j].PutValue($"Row {i+1}, Col {j+1}");
                }
            }

            // PageSetup-Objekt abrufen
            PageSetup pageSetup = worksheet.PageSetup;
            
            // Druckbereich festlegen
            pageSetup.PrintArea = "A1:J100";
            
            // FitToPagesTall-Eigenschaft setzen, um alle Zeilen auf einer Seite zu platzieren
            pageSetup.FitToPagesTall = 1;
            
            // FitToPagesWide-Eigenschaft setzen, um alle Spalten auf einer Seite zu platzieren
            pageSetup.FitToPagesWide = 1;
            
            // Papiergröße festlegen
            pageSetup.PaperSize = PaperSizeType.PaperLetter;
            
            // Rasterlinien drucken
            pageSetup.PrintGridlines = true;

            // Renderoptionen erstellen
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            
            // Blatt-Renderer erstellen
            SheetRender render = new SheetRender(worksheet, options);
            
            // Seitenskalierung ausgeben
            Console.WriteLine($"Page scale: {Math.Round(render.PageScale, 2)}");
        }
    }
}
```

### Siehe auch

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



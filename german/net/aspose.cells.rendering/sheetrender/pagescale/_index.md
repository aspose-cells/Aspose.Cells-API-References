---
title: "SheetRender.PageScale"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SheetRender-Eigenschaft. Gibt den berechneten Seitenskalierungsfaktor des Blatts zurück. Gibt den festgelegten Skalierungswert zurück, wenn Zoom gesetzt ist. Andernfalls wird der berechnete Skalierungswert gemäß FitToPagesWide und FitToPagesTall zurückgegeben"
type: docs
url: /de/net/aspose.cells.rendering/sheetrender/pagescale/
---
## SheetRender.PageScale property

Gibt den berechneten Seitenskalierungsfaktor des Blatts zurück. Gibt den festgelegten Skalierungswert zurück, wenn [`Zoom`](../../../aspose.cells/pagesetup/zoom/) gesetzt ist. Andernfalls wird der berechnete Skalierungswert gemäß [`FitToPagesWide`](../../../aspose.cells/pagesetup/fittopageswide/) und [`FitToPagesTall`](../../../aspose.cells/pagesetup/fittopagestall/) zurückgegeben.

```csharp
public double PageScale { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class SheetRenderPropertyPageScaleDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch mit Beispieldaten
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Füge Beispieldaten zu Zellen hinzu
            for (int i = 0; i < 10; i++)
            {
                sheet.Cells[i, 0].PutValue($"Item {i + 1}");
                sheet.Cells[i, 1].PutValue((i + 1) * 10);
            }

            // Bild- oder Druckoptionen erstellen
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            
            // SheetRender erstellen
            SheetRender sheetRender = new SheetRender(sheet, options);
            
            // Abrufen und Anzeigen der berechneten Seitenskala
            double pageScale = sheetRender.PageScale;
            Console.WriteLine($"Calculated Page Scale: {pageScale}");
        }
    }
}
```

### Siehe auch

* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)



---
title: "ImageOrPrintOptions.OnePagePerSheet"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ImageOrPrintOptions-Eigenschaft. Wenn OnePagePerSheet true ist, wird der gesamte Inhalt eines Blatts nur auf einer Seite im Ergebnis ausgegeben. Die Papiergröße von pagesetup wird ungültig sein und die anderen Einstellungen von pagesetup bleiben weiterhin wirksam."
type: docs
url: /de/net/aspose.cells.rendering/imageorprintoptions/onepagepersheet/
---
## ImageOrPrintOptions.OnePagePerSheet property

Ist OnePagePerSheet true, wird der gesamte Inhalt eines Blatts im Ergebnis nur auf einer Seite ausgegeben. Die Papiergröße der Seiten­einstellungen wird ungültig, während die anderen Einstellungen der Seiten­einstellungen weiterhin wirksam bleiben.

```csharp
public bool OnePagePerSheet { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsPropertyOnePagePerSheetDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Füge Beispieldaten zu Zellen hinzu
            worksheet.Cells["A1"].PutValue("Sample Data for OnePagePerSheet Demo");
            for (int i = 1; i <= 10; i++)
            {
                worksheet.Cells["A" + (i + 1)].PutValue("Row " + i);
            }

            // Bild- oder Druckoptionen erstellen
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.OnePagePerSheet = true; // Key property being demonstrated
            options.ImageType = Aspose.Cells.Drawing.ImageType.Png;
            
            // SheetRender erstellen
            SheetRender sr = new SheetRender(worksheet, options);
            
            // Speichere das Ausgabebild
            sr.ToImage(0, "OnePagePerSheetOutput.png");
            
            Console.WriteLine("Output saved with OnePagePerSheet=true");
        }
    }
}
```

### Siehe auch

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)



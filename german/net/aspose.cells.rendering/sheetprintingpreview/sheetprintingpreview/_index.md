---
title: "SheetPrintingPreview.SheetPrintingPreview"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SheetPrintingPreview-Konstruktor. Die Konstruktion von SheetPrintingPreview"
type: docs
url: /de/net/aspose.cells.rendering/sheetprintingpreview/sheetprintingpreview/
---
## SheetPrintingPreview constructor

Der Aufbau von SheetPrintingPreview

```csharp
public SheetPrintingPreview(Worksheet sheet, ImageOrPrintOptions options)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Blatt | Arbeitsblatt | Geben Sie an, welche Tabelle gedruckt werden soll. |
| Optionen | ImageOrPrintOptions | ImageOrPrintOptions enthält einige Eigenschaften der Ausgabe |

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class SheetPrintingPreviewMethodctorWithWorksheetImageOrPrintOptionsDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Beispieldaten zum Arbeitsblatt hinzufügen
            for (int i = 0; i < 10; i++)
            {
                for (int j = 0; j < 5; j++)
                {
                    worksheet.Cells[i, j].PutValue($"Data {i},{j}");
                }
            }

            // Bild-/Druckoptionen erstellen
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.PrintingPage = PrintingPageType.Default;

            // Sheet-Druckvorschau erstellen
            SheetPrintingPreview preview = new SheetPrintingPreview(worksheet, options);
            
            // Geben Sie die ausgewertete Seitenzahl aus
            Console.WriteLine($"Evaluated page count: {preview.EvaluatedPageCount}");
        }
    }
}
```

### Siehe auch

* class [Worksheet](../../../aspose.cells/worksheet/)
* class [ImageOrPrintOptions](../../imageorprintoptions/)
* class [SheetPrintingPreview](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)



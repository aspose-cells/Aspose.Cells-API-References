---
title: "Worksheet.GetPrintingPageBreaks"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Worksheet-Methode. Gibt automatische Seitenumbrüche zurück"
type: docs
url: /de/net/aspose.cells/worksheet/getprintingpagebreaks/
---
## Worksheet.GetPrintingPageBreaks method

Liest automatische Seitenumbrüche.

```csharp
public CellArea[] GetPrintingPageBreaks(ImageOrPrintOptions options)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Optionen | ImageOrPrintOptions | Die Druckoptionen |

### Rückgabewert

Die automatischen Seitenumbruchbereiche.

### Hinweise

Jeder Zellbereich stellt ein Blatt Papier dar.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class WorksheetMethodGetPrintingPageBreaksWithImageOrPrintOptionsDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Füge Beispieldaten hinzu, um Seitenumbrüche zu erzeugen
            for (int i = 0; i < 100; i++)
            {
                worksheet.Cells[$"A{i+1}"].PutValue($"Row {i+1}");
            }

            // Lege den Druckbereich und die Seiteneinrichtung fest
            worksheet.PageSetup.PrintArea = "A1:A100";
            worksheet.PageSetup.FitToPagesTall = 1;
            worksheet.PageSetup.FitToPagesWide = 1;

            // Erhalte Seitenumbrüche mit ImageOrPrintOptions
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            CellArea[] pageBreaks = worksheet.GetPrintingPageBreaks(options);

            // Gib die Informationen zum ersten Seitenumbruch aus
            Console.WriteLine($"First page break ends at row: {pageBreaks[0].EndRow}");
        }
    }
}
```

### Siehe auch

* struct [CellArea](../../cellarea/)
* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



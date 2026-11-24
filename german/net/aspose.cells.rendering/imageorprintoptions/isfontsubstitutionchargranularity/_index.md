---
title: "ImageOrPrintOptions.IsFontSubstitutionCharGranularity"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ImageOrPrintOptions-Eigenschaft. Gibt an, ob die Schriftart eines Zeichens nur ersetzt werden soll, wenn die Zellen-Schriftart nicht kompatibel ist."
type: docs
url: /de/net/aspose.cells.rendering/imageorprintoptions/isfontsubstitutionchargranularity/
---
## ImageOrPrintOptions.IsFontSubstitutionCharGranularity property

Gibt an, ob die Schriftart eines Zeichens nur dann ersetzt werden soll, wenn die Zellen‑Schriftart nicht kompatibel ist.

```csharp
public bool IsFontSubstitutionCharGranularity { get; set; }
```

### Hinweise

Standard ist false. Wir versuchen zuerst die Standardschriftart des Arbeitsbuchs und von PdfSaveOption/System für die Zellen-Schriftart.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing; // Added missing namespace AsposeCellsExamples
    using Aspose.Cells.Rendering;
    using System;

    public class ImageOrPrintOptionsPropertyIsFontSubstitutionCharGranularityDemo
    {
        public static void Run()
        {
            // Erstelle eine neue Arbeitsmappe und greife auf das erste Arbeitsblatt zu
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Zelle mit potenziell nicht unterstützter Schriftart konfigurieren
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Text with unavailable font");
            Style style = cell.GetStyle();
            style.Font.Name = "NonExistentFont";
            cell.SetStyle(style);

            // Bildrenderoptionen erstellen
            ImageOrPrintOptions options = new ImageOrPrintOptions
            {
                ImageType = ImageType.Png, // Namespace reference now valid
                DefaultFont = "Arial",
                CheckWorkbookDefaultFont = false
            };

            // Eigenschaftswert anzeigen und ändern
            Console.WriteLine($"Initial IsFontSubstitutionCharGranularity: {options.IsFontSubstitutionCharGranularity}");
            
            // Mit der Standardeinstellung rendern
            new SheetRender(worksheet, options).ToImage(0, "BeforeFontSubstitutionChange.png");

            // Eigenschaft ändern und erneut rendern
            options.IsFontSubstitutionCharGranularity = true;
            Console.WriteLine($"Updated IsFontSubstitutionCharGranularity: {options.IsFontSubstitutionCharGranularity}");
            new SheetRender(worksheet, options).ToImage(0, "AfterFontSubstitutionChange.png");

            // Arbeitsmappe zum Referenzieren speichern
            workbook.Save("FontSubstitutionDemoWorkbook.xlsx");
        }
    }
}
```

### Siehe auch

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)



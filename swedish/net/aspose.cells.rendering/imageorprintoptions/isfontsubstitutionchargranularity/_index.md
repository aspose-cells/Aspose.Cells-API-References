---
title: "ImageOrPrintOptions.IsFontSubstitutionCharGranularity"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ImageOrPrintOptions-egenskap. Anger om endast teckensnittet för tecknet ska ersättas när cellens teckensnitt inte är kompatibelt med det"
type: docs
url: /sv/net/aspose.cells.rendering/imageorprintoptions/isfontsubstitutionchargranularity/
---
## ImageOrPrintOptions.IsFontSubstitutionCharGranularity property

Anger om endast teckensnittet för tecknet ska ersättas när cellens teckensnitt inte är kompatibelt.

```csharp
public bool IsFontSubstitutionCharGranularity { get; set; }
```

### Anmärkningar

Standard är false. Vi kommer först att prova standardteckensnittet för Workbook och PdfSaveOption/system för cellens teckensnitt.

### Exempel

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
            // Skapa en ny arbetsbok och öppna det första kalkylbladet
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Konfigurera cell med potentiellt ej stödd teckensnitt
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Text with unavailable font");
            Style style = cell.GetStyle();
            style.Font.Name = "NonExistentFont";
            cell.SetStyle(style);

            // Skapa alternativ för bildrendering
            ImageOrPrintOptions options = new ImageOrPrintOptions
            {
                ImageType = ImageType.Png, // Namespace reference now valid
                DefaultFont = "Arial",
                CheckWorkbookDefaultFont = false
            };

            // Visa och ändra egenskapsvärde
            Console.WriteLine($"Initial IsFontSubstitutionCharGranularity: {options.IsFontSubstitutionCharGranularity}");
            
            // Rendera med standardinställning
            new SheetRender(worksheet, options).ToImage(0, "BeforeFontSubstitutionChange.png");

            // Ändra egenskap och rendera igen
            options.IsFontSubstitutionCharGranularity = true;
            Console.WriteLine($"Updated IsFontSubstitutionCharGranularity: {options.IsFontSubstitutionCharGranularity}");
            new SheetRender(worksheet, options).ToImage(0, "AfterFontSubstitutionChange.png");

            // Spara arbetsbok för referens
            workbook.Save("FontSubstitutionDemoWorkbook.xlsx");
        }
    }
}
```

### Se även

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)



---
title: "Klass AutoFitterOptions"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.AutoFitterOptions klass. Representerar alla auto‑fitter‑alternativ"
type: docs
url: /sv/net/aspose.cells/autofitteroptions/
---
## AutoFitterOptions class

Representerar alla autofit-alternativ.

```csharp
public class AutoFitterOptions
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [AutoFitterOptions](autofitteroptions/)() | Standardkonstruktorn. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [AutoFitMergedCells](../../aspose.cells/autofitteroptions/autofitmergedcells/) { get; set; } | (**Obsolete.**) Anger om radens höjd automatiskt anpassas när cellerna är sammanslagna i en rad. Standardvärdet är false. |
| [AutoFitMergedCellsType](../../aspose.cells/autofitteroptions/autofitmergedcellstype/) { get; set; } | Hämtar och anger typen av automatisk anpassning av radhöjd för sammanslagna celler. |
| [AutoFitWrappedTextType](../../aspose.cells/autofitteroptions/autofitwrappedtexttype/) { get; set; } | Hämtar och anger typen av automatisk anpassning av radbruten text. |
| [DefaultEditLanguage](../../aspose.cells/autofitteroptions/defaulteditlanguage/) { get; set; } | Hämtar eller anger standardspråket för redigering. |
| [FormatStrategy](../../aspose.cells/autofitteroptions/formatstrategy/) { get; set; } | Hämtar och anger den formaterade strategin. |
| [ForRendering](../../aspose.cells/autofitteroptions/forrendering/) { get; set; } | Anger om anpassning för renderingsändamål. |
| [IgnoreHidden](../../aspose.cells/autofitteroptions/ignorehidden/) { get; set; } | Ignorerar dolda rader/kolumner. |
| [MaxRowHeight](../../aspose.cells/autofitteroptions/maxrowheight/) { get; set; } | Hämtar och anger maximal radhöjd (i enheten Point) vid automatisk anpassning av rader. |
| [OnlyAuto](../../aspose.cells/autofitteroptions/onlyauto/) { get; set; } | Anger om endast rader vars höjd inte är anpassad ska anpassas. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;

    public class AutoFitterOptionsDemo
    {
        public static void AutoFitterOptionsExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till lite exempeldata
            worksheet.Cells["A1"].PutValue("This is a sample text that will be wrapped and autofitted.");

            Style style = worksheet.Cells["A1"].GetStyle();

            style.IsTextWrapped = true;

            worksheet.Cells["A1"].SetStyle(style);

            // Skapa ett område A1:B2
            Range range = worksheet.Cells.CreateRange(0, 0, 2, 2);

            // Sammanfoga cellerna
            range.Merge();

            // Skapa en instans av AutoFitterOptions
            AutoFitterOptions options = new AutoFitterOptions
            {
                DefaultEditLanguage = DefaultEditLanguage.English,
                AutoFitMergedCellsType = AutoFitMergedCellsType.EachLine,
                OnlyAuto = true,
                IgnoreHidden = true,
                MaxRowHeight = 50.0,
                AutoFitWrappedTextType = AutoFitWrappedTextType.Paragraph,
                FormatStrategy = CellValueFormatStrategy.DisplayString,
                ForRendering = true
            };

            // Tillämpa automatisk anpassning av rader med de angivna alternativen
            worksheet.AutoFitRows(options);

            // Spara arbetsboken
            workbook.Save("AutoFitterOptionsExample.xlsx");
            workbook.Save("AutoFitterOptionsExample.pdf");

            return;
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)



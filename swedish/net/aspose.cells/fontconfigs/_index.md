---
title: "Klass FontConfigs"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.FontConfigs-klass. Anger teckensnittsinställningar"
type: docs
url: /sv/net/aspose.cells/fontconfigs/
---
## FontConfigs class

Anger teckensnittsinställningar

```csharp
public class FontConfigs
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [FontConfigs](fontconfigs/)() | Standardkonstruktorn. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| static [DefaultFontName](../../aspose.cells/fontconfigs/defaultfontname/) { get; set; } | Hämtar eller anger standardteckensnittets namn. |
| static [PreferSystemFontSubstitutes](../../aspose.cells/fontconfigs/prefersystemfontsubstitutes/) { get; set; } | Indikera om systemets teckensnittssubstitut ska användas först eller inte när ett teckensnitt inte finns tillgängligt och substitutet för detta teckensnitt inte är angivet. t.ex. På Ubuntu ersätts teckensnittet \"Arial\" vanligtvis av \"Liberation Sans\". Standardvärdet är falskt. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| static [GetFontFileDataInfo](../../aspose.cells/fontconfigs/getfontfiledatainfo/)(string, bool, bool, bool) | Hämta datainformation för teckensnittsfilens data. |
| static [GetFontSources](../../aspose.cells/fontconfigs/getfontsources/)() | Hämtar en kopia av arrayen som innehåller listan över källor |
| static [GetFontSubstitutes](../../aspose.cells/fontconfigs/getfontsubstitutes/)(string) | Returnerar en array som innehåller namn på teckensnittssubstitut som ska användas om originalteckensnittet saknas. |
| static [IsFontAvailable](../../aspose.cells/fontconfigs/isfontavailable/)(string) | Indikera om teckensnittet är tillgängligt. |
| static [SetFontFolder](../../aspose.cells/fontconfigs/setfontfolder/)(string, bool) | Anger teckensnittsmappen |
| static [SetFontFolders](../../aspose.cells/fontconfigs/setfontfolders/)(string[], bool) | Anger teckensnittsmappen |
| static [SetFontSources](../../aspose.cells/fontconfigs/setfontsources/)(FontSourceBase[]) | Anger teckensnittskällorna. |
| static [SetFontSubstitutes](../../aspose.cells/fontconfigs/setfontsubstitutes/)(string, string[]) | Namn på teckensnittssubstitut för angivet originalteckensnitt. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassFontConfigsDemo
    {
        public static void Run()
        {
            // Ange anpassad teckensnittsmapp
            string fontFolder = @"C:\MyFonts\";
            FontConfigs.SetFontFolder(fontFolder, true);

            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ange exempeltext med olika teckensnitt
            worksheet.Cells["A1"].PutValue("Text with default font");
            worksheet.Cells["A2"].PutValue("Text with custom font");
            
            // Tillämpa anpassad teckensnittsstil
            Style style = workbook.CreateStyle();
            style.Font.Name = "MyCustomFont"; // This font should exist in the custom font folder
            worksheet.Cells["A2"].SetStyle(style);

            // Spara till HTML för att demonstrera teckensnittsrendering
            HtmlSaveOptions options = new HtmlSaveOptions
            {
                ExportImagesAsBase64 = true,
                PresentationPreference = true
            };
            
            workbook.Save("output.html", options);
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)



---
title: "Klass IndividualFontConfigs"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.IndividualFontConfigs-klass. Teckensnittskonfigurationer för varje Workbook-objekt"
type: docs
url: /sv/net/aspose.cells/individualfontconfigs/
---
## IndividualFontConfigs class

Teckensnittskonfigurationer för varje [`Workbook`](../workbook/) objekt.

```csharp
public class IndividualFontConfigs
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [IndividualFontConfigs](individualfontconfigs/)() | Konstruktor. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [GetFontSources](../../aspose.cells/individualfontconfigs/getfontsources/)() | Hämtar en kopia av arrayen som innehåller listan över källor |
| [GetFontSubstitutes](../../aspose.cells/individualfontconfigs/getfontsubstitutes/)(string) | Returnerar en array som innehåller teckensnittsersättningsnamn som ska användas om originalteckensnittet inte finns. |
| [SetFontFolder](../../aspose.cells/individualfontconfigs/setfontfolder/)(string, bool) | Anger teckensnittsmappen |
| [SetFontFolders](../../aspose.cells/individualfontconfigs/setfontfolders/)(string[], bool) | Ställer in teckensnittsmapparna |
| [SetFontSources](../../aspose.cells/individualfontconfigs/setfontsources/)(FontSourceBase[]) | Anger teckensnittskällorna. |
| [SetFontSubstitutes](../../aspose.cells/individualfontconfigs/setfontsubstitutes/)(string, string[]) | Ställer in teckensnittsersättningsnamn för ett givet originalteckensnittsnamn. |

### Exempel

```csharp
using System;
using System.IO;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassIndividualFontConfigsDemo
    {
        public static void Run()
        {
            // Skapa tillfälliga kataloger för teckensnittskällor
            string tempFontFolder1 = Path.Combine(Path.GetTempPath(), "FontFolder1_" + Guid.NewGuid().ToString());
            string tempFontFolder2 = Path.Combine(Path.GetTempPath(), "FontFolder2_" + Guid.NewGuid().ToString());
            Directory.CreateDirectory(tempFontFolder1);
            Directory.CreateDirectory(tempFontFolder2);

            // Skapa exempel CSV-fil
            string csvFilePath = "sample_data.csv";
            File.WriteAllText(csvFilePath, "Name,Age\nJohn,30\nAlice,25", Encoding.UTF8);

            try
            {
                // Initiera teckensnittskonfiguration
                IndividualFontConfigs fontConfigs = new IndividualFontConfigs();

                // Ställ in teckensnittssubstitut för Arial
                fontConfigs.SetFontSubstitutes("Arial", new string[] { "Times New Roman", "Verdana" });

                // Konfigurera teckensnittskataloger
                fontConfigs.SetFontFolder(tempFontFolder1, false);
                fontConfigs.SetFontFolders(new string[] { tempFontFolder1, tempFontFolder2 }, true);

                // Konfigurera teckensnittskällor
                FontSourceBase[] fontSources = {
                    new FolderFontSource(tempFontFolder1, false),
                    new FolderFontSource(tempFontFolder2, true)
                };
                fontConfigs.SetFontSources(fontSources);

                // Skapa alternativ för textladdning med teckensnittskonfigurationer
                TxtLoadOptions loadOptions = new TxtLoadOptions(LoadFormat.Csv)
                {
                    FontConfigs = fontConfigs
                };

                // Läs in arbetsbok med konfigurerade alternativ
                using (Workbook workbook = new Workbook(csvFilePath, loadOptions))
                {
                    // Spara som Excel-fil
                    workbook.Save("output_with_font_config.xlsx");
                }
            }
            finally
            {
                // Rensa temporära resurser
                if (Directory.Exists(tempFontFolder1)) Directory.Delete(tempFontFolder1, true);
                if (Directory.Exists(tempFontFolder2)) Directory.Delete(tempFontFolder2, true);
                if (File.Exists(csvFilePath)) File.Delete(csvFilePath);
            }
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)



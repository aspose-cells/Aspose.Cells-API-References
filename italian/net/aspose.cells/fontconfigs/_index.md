---
title: "Classe FontConfigs"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.FontConfigs. Specifica le impostazioni del carattere"
type: docs
url: /it/net/aspose.cells/fontconfigs/
---
## FontConfigs class

Specifica le impostazioni del font

```csharp
public class FontConfigs
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [FontConfigs](fontconfigs/)() | Il costruttore predefinito. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| static [DefaultFontName](../../aspose.cells/fontconfigs/defaultfontname/) { get; set; } | Ottiene o imposta il nome del carattere predefinito. |
| static [PreferSystemFontSubstitutes](../../aspose.cells/fontconfigs/prefersystemfontsubstitutes/) { get; set; } | Indica se utilizzare prima le sostituzioni di caratteri di sistema o meno quando un carattere non è presente e la sostituzione di questo carattere non è impostata. Ad esempio, su Ubuntu, il carattere "Arial" è generalmente sostituito da "Liberation Sans". Il valore predefinito è false. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| static [GetFontFileDataInfo](../../aspose.cells/fontconfigs/getfontfiledatainfo/)(string, bool, bool, bool) | Ottieni le informazioni sui dati del file del carattere. |
| static [GetFontSources](../../aspose.cells/fontconfigs/getfontsources/)() | Ottiene una copia dell'array che contiene l'elenco delle fonti. |
| static [GetFontSubstitutes](../../aspose.cells/fontconfigs/getfontsubstitutes/)(string) | Restituisce un array contenente i nomi delle sostituzioni di carattere da utilizzare se il carattere originale non è presente. |
| static [IsFontAvailable](../../aspose.cells/fontconfigs/isfontavailable/)(string) | Indica se il carattere è disponibile. |
| static [SetFontFolder](../../aspose.cells/fontconfigs/setfontfolder/)(string, bool) | Imposta la cartella dei caratteri |
| static [SetFontFolders](../../aspose.cells/fontconfigs/setfontfolders/)(string[], bool) | Imposta la cartella dei caratteri |
| static [SetFontSources](../../aspose.cells/fontconfigs/setfontsources/)(FontSourceBase[]) | Imposta le fonti dei caratteri. |
| static [SetFontSubstitutes](../../aspose.cells/fontconfigs/setfontsubstitutes/)(string, string[]) | Nomi delle sostituzioni di carattere per il nome del carattere originale fornito. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassFontConfigsDemo
    {
        public static void Run()
        {
            // Imposta la cartella dei caratteri personalizzata
            string fontFolder = @"C:\MyFonts\";
            FontConfigs.SetFontFolder(fontFolder, true);

            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Imposta il testo di esempio con diversi caratteri
            worksheet.Cells["A1"].PutValue("Text with default font");
            worksheet.Cells["A2"].PutValue("Text with custom font");
            
            // Applica lo stile di carattere personalizzato
            Style style = workbook.CreateStyle();
            style.Font.Name = "MyCustomFont"; // This font should exist in the custom font folder
            worksheet.Cells["A2"].SetStyle(style);

            // Salva in HTML per dimostrare il rendering dei caratteri
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

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)



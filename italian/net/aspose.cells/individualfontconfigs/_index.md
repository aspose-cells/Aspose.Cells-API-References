---
title: "Classe IndividualFontConfigs"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.IndividualFontConfigs. Configurazioni dei caratteri per ogni oggetto Workbook"
type: docs
url: /it/net/aspose.cells/individualfontconfigs/
---
## IndividualFontConfigs class

Configurazioni dei caratteri per ogni oggetto [`Workbook`](../workbook/).

```csharp
public class IndividualFontConfigs
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [IndividualFontConfigs](individualfontconfigs/)() | Ctor. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [GetFontSources](../../aspose.cells/individualfontconfigs/getfontsources/)() | Ottiene una copia dell'array che contiene l'elenco delle fonti. |
| [GetFontSubstitutes](../../aspose.cells/individualfontconfigs/getfontsubstitutes/)(string) | Restituisce un array contenente i nomi dei caratteri sostitutivi da utilizzare se il carattere originale non è presente. |
| [SetFontFolder](../../aspose.cells/individualfontconfigs/setfontfolder/)(string, bool) | Imposta la cartella dei caratteri |
| [SetFontFolders](../../aspose.cells/individualfontconfigs/setfontfolders/)(string[], bool) | Imposta le cartelle dei caratteri |
| [SetFontSources](../../aspose.cells/individualfontconfigs/setfontsources/)(FontSourceBase[]) | Imposta le fonti dei caratteri. |
| [SetFontSubstitutes](../../aspose.cells/individualfontconfigs/setfontsubstitutes/)(string, string[]) | Imposta i nomi dei caratteri sostitutivi per un dato nome di carattere originale. |

### Esempi

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
            // Crea directory temporanee per le font di origine.
            string tempFontFolder1 = Path.Combine(Path.GetTempPath(), "FontFolder1_" + Guid.NewGuid().ToString());
            string tempFontFolder2 = Path.Combine(Path.GetTempPath(), "FontFolder2_" + Guid.NewGuid().ToString());
            Directory.CreateDirectory(tempFontFolder1);
            Directory.CreateDirectory(tempFontFolder2);

            // Crea file CSV di esempio
            string csvFilePath = "sample_data.csv";
            File.WriteAllText(csvFilePath, "Name,Age\nJohn,30\nAlice,25", Encoding.UTF8);

            try
            {
                // Inizializza la configurazione dei caratteri
                IndividualFontConfigs fontConfigs = new IndividualFontConfigs();

                // Imposta i sostituti dei caratteri per Arial
                fontConfigs.SetFontSubstitutes("Arial", new string[] { "Times New Roman", "Verdana" });

                // Configura le directory dei caratteri
                fontConfigs.SetFontFolder(tempFontFolder1, false);
                fontConfigs.SetFontFolders(new string[] { tempFontFolder1, tempFontFolder2 }, true);

                // Configura le font di origine
                FontSourceBase[] fontSources = {
                    new FolderFontSource(tempFontFolder1, false),
                    new FolderFontSource(tempFontFolder2, true)
                };
                fontConfigs.SetFontSources(fontSources);

                // Crea opzioni di caricamento del testo con configurazioni dei font
                TxtLoadOptions loadOptions = new TxtLoadOptions(LoadFormat.Csv)
                {
                    FontConfigs = fontConfigs
                };

                // Carica la cartella di lavoro con le opzioni configurate
                using (Workbook workbook = new Workbook(csvFilePath, loadOptions))
                {
                    // Salva come file Excel
                    workbook.Save("output_with_font_config.xlsx");
                }
            }
            finally
            {
                // Pulisci le risorse temporanee
                if (Directory.Exists(tempFontFolder1)) Directory.Delete(tempFontFolder1, true);
                if (Directory.Exists(tempFontFolder2)) Directory.Delete(tempFontFolder2, true);
                if (File.Exists(csvFilePath)) File.Delete(csvFilePath);
            }
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)



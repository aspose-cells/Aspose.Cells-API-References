---
title: "LowCodeSaveOptionsProviderOfPlaceHolders.BuildPathWithSheetAlways"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà LowCodeSaveOptionsProviderOfPlaceHolders. Indica se aggiungere sempre l'indice o il nome del foglio al percorso del file. Il valore predefinito è false, cioè quando c'è solo un foglio l'indice e il nome del foglio e il prefisso corrispondente SheetNamePrefix non verranno aggiunti al percorso del file."
type: docs
url: /it/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/buildpathwithsheetalways/
---
## LowCodeSaveOptionsProviderOfPlaceHolders.BuildPathWithSheetAlways property

Indica se aggiungere sempre l'indice o il nome del foglio al percorso del file. Il valore predefinito è false, cioè quando c'è solo un foglio, l'indice e il nome del foglio e il prefisso corrispondente ([`SheetNamePrefix`](../sheetnameprefix/)) non verranno aggiunti al percorso del file.

```csharp
public bool BuildPathWithSheetAlways { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeSaveOptionsProviderOfPlaceHoldersPropertyBuildPathWithSheetAlwaysDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con due fogli per dimostrare le differenze di percorso
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            
            // Configura il provider con segnaposto per l'indice del foglio
            var provider = new LowCodeSaveOptionsProviderOfPlaceHolders("Output_{sheet_index}.xlsx")
            {
                // Dimostra lo scostamento dell'indice del foglio (opzionale)
                SheetIndexOffset = 1
            };

            Console.WriteLine($"Initial BuildPathWithSheetAlways: {provider.BuildPathWithSheetAlways}");

            // Salva con indice del foglio solo quando ci sono più fogli (comportamento predefinito)
            provider.BuildPathWithSheetAlways = false;
            SaveWithProvider(workbook, provider, "DefaultBehavior");

            // Forza l'indice del foglio nei nomi file anche per fogli singoli
            provider.BuildPathWithSheetAlways = true;
            Console.WriteLine($"Modified BuildPathWithSheetAlways: {provider.BuildPathWithSheetAlways}");
            SaveWithProvider(workbook, provider, "ForcedSheetIndex");
        }

        private static void SaveWithProvider(Workbook workbook, LowCodeSaveOptionsProviderOfPlaceHolders provider, string saveDescription)
        {
            // Configura le opzioni di salvataggio con formato JSON per abilitare la divisione
            var saveOptions = new LowCodeSaveOptions
            {
                SaveFormat = SaveFormat.Json
            };

            // Configura il provider con le opzioni di salvataggio
            provider.SaveOptionsTemplate = saveOptions;

            // Salva con percorsi determinati dal provider
            Console.WriteLine($"Saving with {saveDescription} - check output files");
            workbook.Save($"dummy_{saveDescription}.json", saveOptions.SaveFormat);
        }
    }
}
```

### Vedi anche

* class [LowCodeSaveOptionsProviderOfPlaceHolders](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)



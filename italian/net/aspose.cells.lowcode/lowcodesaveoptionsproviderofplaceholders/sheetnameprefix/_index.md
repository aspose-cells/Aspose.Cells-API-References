---
title: "LowCodeSaveOptionsProviderOfPlaceHolders.SheetNamePrefix"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà LowCodeSaveOptionsProviderOfPlaceHolders. Prefisso per l'indice del foglio di lavoro"
type: docs
url: /it/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/sheetnameprefix/
---
## LowCodeSaveOptionsProviderOfPlaceHolders.SheetNamePrefix property

Prefisso per l'indice del foglio di lavoro.

```csharp
public string SheetNamePrefix { get; set; }
```

### Osservazioni

Se c'è solo un foglio di lavoro e [`BuildPathWithSheetAlways`](../buildpathwithsheetalways/) è false, allora questo prefisso e l'indice del foglio (o nome) non verranno aggiunti al percorso del file risultante.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeSaveOptionsProviderOfPlaceHoldersPropertySheetNamePrefixDemo
    {
        public static void Run()
        {
            // Crea una nuova cartella di lavoro con due fogli di lavoro
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Name = "SalesData";
            workbook.Worksheets.Add("FinancialReport");

            // Inizializza il provider con un modello di percorso contenente il segnaposto del foglio
            string pathTemplate = "output_{sheet}.xlsx";
            var provider = new LowCodeSaveOptionsProviderOfPlaceHolders(pathTemplate);

            // Mostra il valore iniziale di SheetNamePrefix (vuoto per impostazione predefinita)
            Console.WriteLine("Initial SheetNamePrefix: " + provider.SheetNamePrefix);

            // Imposta un nuovo prefisso e assicurati che la generazione del percorso includa le informazioni del foglio
            provider.SheetNamePrefix = "Q4_";
            provider.BuildPathWithSheetAlways = true;

            // Configura le opzioni di salvataggio con il formato corretto
            provider.SaveOptionsTemplate = new LowCodeSaveOptions
            {
                SaveFormat = SaveFormat.Xlsx // Set the correct save format
            };

            // Salva la cartella di lavoro usando il provider - genera "output_Q4_SalesData.xlsx" e "output_Q4_FinancialReport.xlsx"
            workbook.Save("result_directory", SaveFormat.Xlsx); // Pass correct SaveFormat
        }
    }
}
```

### Vedi anche

* class [LowCodeSaveOptionsProviderOfPlaceHolders](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)



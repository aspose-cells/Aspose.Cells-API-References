---
title: "LowCodeSaveOptionsProviderOfPlaceHolders.SplitPartPrefix"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà LowCodeSaveOptionsProviderOfPlaceHolders. Prefisso per l'indice della parte divisa"
type: docs
url: /it/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/splitpartprefix/
---
## LowCodeSaveOptionsProviderOfPlaceHolders.SplitPartPrefix property

Prefisso per l'indice della parte divisa.

```csharp
public string SplitPartPrefix { get; set; }
```

### Osservazioni

Se c'è una sola parte divisa e [`BuildPathWithSplitPartAlways`](../buildpathwithsplitpartalways/) è false, allora questo prefisso e l'indice della parte divisa (0) non verranno aggiunti al percorso del file risultante.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeSaveOptionsProviderOfPlaceHoldersPropertySplitPartPrefixDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            for (int i = 0; i < 25; i++)
            {
                worksheet.Cells[i, 0].Value = $"Data row {i + 1}";
            }

            // Configura il modello delle opzioni di salvataggio
            LowCodeSaveOptions saveOptionsTemplate = new LowCodeSaveOptions();

            // Inizializza il provider con il segnaposto della parte divisa
            LowCodeSaveOptionsProviderOfPlaceHolders provider = new LowCodeSaveOptionsProviderOfPlaceHolders("SplitResult_Sheet{sheet}_Part{split}.xlsx")
            {
                SaveOptionsTemplate = saveOptionsTemplate
            };

            // Mostra e modifica SplitPartPrefix
            Console.WriteLine($"Initial SplitPartPrefix: {provider.SplitPartPrefix}");
            provider.SplitPartPrefix = "Section";
            Console.WriteLine($"Updated SplitPartPrefix: {provider.SplitPartPrefix}");

            // Salva la cartella di lavoro con parti divise usando il formato di salvataggio del provider
            workbook.Save("output", saveOptionsTemplate.SaveFormat);

            Console.WriteLine("Check 'output' directory for split files with 'Section' prefix");
        }
    }
}
```

### Vedi anche

* class [LowCodeSaveOptionsProviderOfPlaceHolders](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)



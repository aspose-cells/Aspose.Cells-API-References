---
title: "LowCodeSaveOptionsProviderOfPlaceHolders.BuildPathWithSplitPartAlways"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà LowCodeSaveOptionsProviderOfPlaceHolders. Indica se aggiungere sempre l'indice della parte divisa al percorso del file. Il valore predefinito è false, cioè quando c'è solo una parte divisa l'indice della parte divisa e il prefisso corrispondente SplitPartPrefix non verranno aggiunti al percorso del file."
type: docs
url: /it/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/buildpathwithsplitpartalways/
---
## LowCodeSaveOptionsProviderOfPlaceHolders.BuildPathWithSplitPartAlways property

Indica se aggiungere sempre l'indice della parte divisa al percorso del file. Il valore predefinito è false, cioè quando c'è solo una parte divisa, l'indice della parte divisa e il prefisso corrispondente ([`SplitPartPrefix`](../splitpartprefix/)) non verranno aggiunti al percorso del file.

```csharp
public bool BuildPathWithSplitPartAlways { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeSaveOptionsProviderOfPlaceHoldersPropertyBuildPathWithSplitPartAlwaysDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con dati che non verranno suddivisi in più parti
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Single Part Demonstration";

            // Crea un provider con modello di percorso e condizione di divisione che produce una sola parte
            var provider = new LowCodeSaveOptionsProviderOfPlaceHolders("Result_{split}.xlsx")
            {
                SaveOptionsTemplate = new LowCodeSaveOptions()
            };

            // Dimostra lo stato false della proprietà (predefinito)
            Console.WriteLine($"Initial BuildPathWithSplitPartAlways: {provider.BuildPathWithSplitPartAlways}");
            provider.BuildPathWithSplitPartAlways = false;
            
            // Questo genererebbe Result.xlsx quando esiste una sola parte
            Console.WriteLine("Saving with BuildPathWithSplitPartAlways=false");
            ExecuteDummySave(workbook, "Result.xlsx");

            // Attiva/disattiva la proprietà e dimostra lo stato true
            provider.BuildPathWithSplitPartAlways = true;
            Console.WriteLine("\nSaving with BuildPathWithSplitPartAlways=true");
            
            // Questo genererebbe Result_0.xlsx anche con una singola parte
            ExecuteDummySave(workbook, "Result_0.xlsx");
        }

        private static void ExecuteDummySave(Workbook workbook, string filename)
        {
            // Nell'uso reale, sostituire con l'operazione di salvataggio basata sul provider
            Console.WriteLine($"Simulated save operation -> Filename: {filename}");
            workbook.Save(filename, SaveFormat.Xlsx);
        }
    }
}
```

### Vedi anche

* class [LowCodeSaveOptionsProviderOfPlaceHolders](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)



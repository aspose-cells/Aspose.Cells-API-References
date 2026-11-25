---
title: "LowCodeSaveOptionsProviderOfAssembling.PathHeader"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "LowCodeSaveOptionsProviderOfAssembling property. Intestazione della parte prima del contenuto aggiunto del foglio e della parte divisa del percorso del file"
type: docs
url: /it/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/pathheader/
---
## LowCodeSaveOptionsProviderOfAssembling.PathHeader property

Parte intestazione (prima del contenuto aggiunto del foglio e della parte divisa) del percorso del file.

```csharp
public string PathHeader { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeSaveOptionsProviderOfAssemblingPropertyPathHeaderDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con dati che verranno suddivisi in più parti
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            for (int i = 0; i < 150; i++)
            {
                worksheet.Cells[i, 0].Value = $"Data row {i + 1}";
            }

            // Inizializza il provider delle opzioni di salvataggio con i valori predefiniti
            var provider = new LowCodeSaveOptionsProviderOfAssembling
            {
                PathHeader = "output/QuarterlyReport_",
                PathTail = ".html",
                UseSheetName = true,
                SaveOptionsTemplate = new LowCodeSaveOptions() // Changed from HtmlSaveOptions to LowCodeSaveOptions
            };

            Console.WriteLine($"Initial PathHeader: {provider.PathHeader}");

            // Modifica la configurazione del percorso
            provider.PathHeader = "output/ModifiedReport_";
            provider.SheetPrefix = "Sheet_";
            provider.SplitPartPrefix = "Part_";

            // Dimostra l'effetto salvando con la configurazione corrente del provider
            workbook.Save("result.html", SaveFormat.Html); // Changed second parameter to SaveFormat.Html

            Console.WriteLine("Check 'output' directory for split files named like 'ModifiedReport_Sheet_0_Part_0.html'");
        }
    }
}
```

### Vedi anche

* class [LowCodeSaveOptionsProviderOfAssembling](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)



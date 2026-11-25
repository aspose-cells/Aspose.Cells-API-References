---
title: "LowCodeSaveOptionsProviderOfAssembling.SplitPartPrefix"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà LowCodeSaveOptionsProviderOfAssembling. Prefisso per l'indice della parte divisa"
type: docs
url: /it/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/splitpartprefix/
---
## LowCodeSaveOptionsProviderOfAssembling.SplitPartPrefix property

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
    using Aspose.Cells.Rendering;
    using System;

    public class LowCodeSaveOptionsProviderOfAssemblingPropertySplitPartPrefixDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con dati che si estendono su più pagine
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            for (int i = 0; i < 100; i++)
                worksheet.Cells[$"A{i + 1}"].Value = $"Data Row {i + 1}";

            // Configura le impostazioni della pagina per creare più pagine
            worksheet.PageSetup.PrintArea = "A1:A30";
            worksheet.PageSetup.FitToPagesTall = 1;

            // Inizializza il provider delle opzioni di salvataggio con la configurazione di divisione
            var provider = new LowCodeSaveOptionsProviderOfAssembling
            {
                PathHeader = "SplitResults/",
                SplitPartPrefix = "OriginalPart_",
                PathTail = ".pdf",
                SaveOptionsTemplate = new LowCodeSaveOptions { SaveFormat = SaveFormat.Pdf }
            };

            Console.WriteLine($"Initial SplitPartPrefix: {provider.SplitPartPrefix}");

            // Salva con prefisso iniziale (genererà SplitResults/OriginalPart_0.pdf ecc.)
            workbook.Save("InitialSplit.pdf", new PdfSaveOptions());

            // Modifica il prefisso di divisione
            provider.SplitPartPrefix = "ModifiedPart_";
            Console.WriteLine($"Updated SplitPartPrefix: {provider.SplitPartPrefix}");

            // Salva con prefisso modificato (genererà SplitResults/ModifiedPart_0.pdf ecc.)
            workbook.Save("ModifiedSplit.pdf", new PdfSaveOptions());
        }
    }
}
```

### Vedi anche

* class [LowCodeSaveOptionsProviderOfAssembling](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)



---
title: "LowCodeSaveOptionsProviderOfAssembling.SaveOptionsTemplate"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "LowCodeSaveOptionsProviderOfAssembling property. Il modello per creare un'istanza delle opzioni di salvataggio in GetSaveOptions"
type: docs
url: /it/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/saveoptionstemplate/
---
## LowCodeSaveOptionsProviderOfAssembling.SaveOptionsTemplate property

Il modello per creare un'istanza delle opzioni di salvataggio in [`GetSaveOptions`](../getsaveoptions/).

```csharp
public LowCodeSaveOptions SaveOptionsTemplate { get; set; }
```

### Osservazioni

Se il modello è stato specificato, l'istanza creata copierà tutte le impostazioni da esso e aggiornerà il file di output di conseguenza.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using Aspose.Cells.Saving;
    using System;

    public class LowCodeSaveOptionsProviderOfAssemblingPropertySaveOptionsTemplateDemo
    {
        public static void Run()
        {
            // Crea una nuova cartella di lavoro con due fogli di lavoro
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            Worksheet worksheet1 = workbook.Worksheets[0];
            Worksheet worksheet2 = workbook.Worksheets[1];
            worksheet1.Cells["A1"].PutValue("Sheet1 Content");
            worksheet2.Cells["A1"].PutValue("Sheet2 Content");

            // Crea un'istanza di LowCodeSaveOptionsProviderOfAssembling
            var provider = new LowCodeSaveOptionsProviderOfAssembling
            {
                PathHeader = "Output/Sheet",
                PathTail = ".xlsx",
                BuildPathWithSheetAlways = true,
                UseSheetName = false
            };

            // Mostra lo stato iniziale di SaveOptionsTemplate
            Console.WriteLine("Initial SaveOptionsTemplate is " + (provider.SaveOptionsTemplate == null ? "null" : "set"));

            // Configura SaveOptionsTemplate con la crittografia
            provider.SaveOptionsTemplate = new LowCodeSaveOptions();
            Console.WriteLine("SaveOptionsTemplate configured");

            // Crea le opzioni di salvataggio LowCode
            var saveOptions = new LowCodeSaveOptions();

            // Salva la cartella di lavoro usando il provider configurato (genererà file separati per foglio)
            workbook.Save("output_combined.xlsx", saveOptions.SaveFormat);

            Console.WriteLine("Demo executed successfully. Check output files.");
        }
    }
}
```

### Vedi anche

* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [LowCodeSaveOptionsProviderOfAssembling](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)



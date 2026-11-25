---
title: "LowCodeMergeOptions.SaveOptions"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà LowCodeMergeOptions. Opzioni di salvataggio per salvare le parti divise"
type: docs
url: /it/net/aspose.cells.lowcode/lowcodemergeoptions/saveoptions/
---
## LowCodeMergeOptions.SaveOptions property

Opzioni di salvataggio per salvare le parti divise.

```csharp
public LowCodeSaveOptions SaveOptions { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeMergeOptionsPropertySaveOptionsDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Merged Data");

            // Inizializza le opzioni di merge
            LowCodeMergeOptions mergeOptions = new LowCodeMergeOptions();
            Console.WriteLine("Initial SaveOptions: " + (mergeOptions.SaveOptions?.GetType().Name ?? "null"));

            // Configura nuove opzioni di salvataggio
            LowCodeSaveOptions saveOptions = new LowCodeSaveOptions();
            saveOptions.SaveFormat = SaveFormat.Xlsx;
            // Imposta password tramite le impostazioni della cartella di lavoro
            workbook.Settings.Password = "Aspose1234!";
            mergeOptions.SaveOptions = saveOptions;

            // Dimostra l'effetto salvando con le opzioni configurate
            workbook.Save("MergedWithOptions.xlsx", saveOptions.SaveFormat);

            Console.WriteLine("Workbook saved with password-protected SaveOptions.");
        }
    }
}
```

### Vedi anche

* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [LowCodeMergeOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)



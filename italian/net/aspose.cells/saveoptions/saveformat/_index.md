---
title: "SaveOptions.SaveFormat"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà SaveOptions. Ottiene il formato del file di salvataggio"
type: docs
url: /it/net/aspose.cells/saveoptions/saveformat/
---
## SaveOptions.SaveFormat property

Ottiene il formato di salvataggio del file.

```csharp
public SaveFormat SaveFormat { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SaveOptionsPropertySaveFormatDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello World!");

            // Dimostra diversi formati di salvataggio
            SaveOptions[] options = {
                new PdfSaveOptions(),
                new OoxmlSaveOptions(),
                new HtmlSaveOptions()
            };

            foreach (var saveOptions in options)
            {
                string extension = FileFormatUtil.SaveFormatToExtension(saveOptions.SaveFormat);
                Console.WriteLine($"Saving as {saveOptions.SaveFormat} with extension: {extension}");

                string outputPath = $"output_{Guid.NewGuid().ToString("N").Substring(0, 8)}{extension}";
                workbook.Save(outputPath, saveOptions);
                Console.WriteLine($"Saved to: {outputPath}");
            }

            // Pulisci
            workbook.Dispose();
        }
    }
}
```

### Vedi anche

* enum [SaveFormat](../../saveformat/)
* class [SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



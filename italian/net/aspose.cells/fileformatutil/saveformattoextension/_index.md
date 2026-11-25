---
title: "FileFormatUtil.SaveFormatToExtension"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo FileFormatUtil. Converte un valore enumerato di formato di salvataggio in un'estensione di file"
type: docs
url: /it/net/aspose.cells/fileformatutil/saveformattoextension/
---
## FileFormatUtil.SaveFormatToExtension method

Converte un valore enumerato di SaveFormat in un'estensione di file.

```csharp
public static string SaveFormatToExtension(SaveFormat format)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| formato | SaveFormat | Il formato di salvataggio. |

### Valore di ritorno

L'estensione restituita è una stringa in minuscolo con un punto iniziale.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FileFormatUtilMethodSaveFormatToExtensionWithSaveFormatDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test content");

            // Dimostrare SaveFormatToExtension con formati diversi
            SaveOptions[] saveOptions = {
                new PdfSaveOptions(),
                new XlsSaveOptions(SaveFormat.Excel97To2003),
                new OoxmlSaveOptions(SaveFormat.Xlsx),
                new OdsSaveOptions()
            };

            foreach (var options in saveOptions)
            {
                string extension = FileFormatUtil.SaveFormatToExtension(options.SaveFormat);
                Console.WriteLine($"SaveFormat: {options.SaveFormat} -> Extension: {extension}");
                
                // Salva con l'estensione rilevata
                string fileName = $"output{extension}";
                workbook.Save(fileName, options);
                Console.WriteLine($"Saved file: {fileName}");
            }

            workbook.Dispose();
        }
    }
}
```

### Vedi anche

* enum [SaveFormat](../../saveformat/)
* class [FileFormatUtil](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



---
title: "FileFormatUtil.LoadFormatToSaveFormat"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo FileFormatUtil. Converte un valore LoadFormat in un valore SaveFormat se possibile"
type: docs
url: /it/net/aspose.cells/fileformatutil/loadformattosaveformat/
---
## FileFormatUtil.LoadFormatToSaveFormat method

Converte un valore LoadFormat in un valore SaveFormat, se possibile.

```csharp
public static SaveFormat LoadFormatToSaveFormat(LoadFormat loadFormat)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| loadFormat | LoadFormat | Il formato di caricamento. |

### Valore di ritorno

Il formato di salvataggio.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FileFormatUtilMethodLoadFormatToSaveFormatWithLoadFormatDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();

            try
            {
                LoadFormat inputFormat = LoadFormat.Xlsx;

                SaveFormat outputFormat = FileFormatUtil.LoadFormatToSaveFormat(inputFormat);
                Console.WriteLine($"Converted LoadFormat.{inputFormat} to SaveFormat.{outputFormat}");

                string fileExtension = FileFormatUtil.SaveFormatToExtension(outputFormat);
                string outputFileName = $"OutputFile_{DateTime.Now.Ticks}.{fileExtension}";
                
                workbook.Save(outputFileName, outputFormat);
                Console.WriteLine($"Workbook saved successfully as: {outputFileName}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during conversion or saving: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* enum [SaveFormat](../../saveformat/)
* enum [LoadFormat](../../loadformat/)
* class [FileFormatUtil](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



---
title: "FileFormatUtil.ExtensionToSaveFormat"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo FileFormatUtil. Converte l'estensione di un nome file in un valore SaveFormat"
type: docs
url: /it/net/aspose.cells/fileformatutil/extensiontosaveformat/
---
## FileFormatUtil.ExtensionToSaveFormat method

Converte l'estensione del nome file in un valore SaveFormat.

```csharp
public static SaveFormat ExtensionToSaveFormat(string extension)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| estensione | String | L'estensione del file. Può essere con o senza il punto iniziale. Non distingue tra maiuscole e minuscole. |

### Osservazioni

Se l'estensione non può essere riconosciuta, restituisce Unknown.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FileFormatUtilMethodExtensionToSaveFormatWithStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("File format demonstration");

            try
            {
                string fileExtension = ".xlsx";
                
                SaveFormat saveFormat = FileFormatUtil.ExtensionToSaveFormat(fileExtension);
                Console.WriteLine($"File extension '{fileExtension}' maps to SaveFormat: {saveFormat}");
                
                string verifiedExtension = FileFormatUtil.SaveFormatToExtension(saveFormat);
                string outputPath = $"ExtensionConversionDemo{verifiedExtension}";
                
                workbook.Save(outputPath, saveFormat);
                Console.WriteLine($"Workbook saved successfully in {saveFormat} format");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during format conversion: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* enum [SaveFormat](../../saveformat/)
* class [FileFormatUtil](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



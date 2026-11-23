---
title: "FileFormatUtil.ExtensionToSaveFormat"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode FileFormatUtil. Convertit une extension de nom de fichier en une valeur SaveFormat"
type: docs
url: /fr/net/aspose.cells/fileformatutil/extensiontosaveformat/
---
## FileFormatUtil.ExtensionToSaveFormat method

Convertit une extension de nom de fichier en valeur SaveFormat.

```csharp
public static SaveFormat ExtensionToSaveFormat(string extension)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| extension | String | L'extension du fichier. Peut être avec ou sans point initial. Insensible à la casse. |

### Remarques

Si l'extension ne peut pas être reconnue, renvoie Unknown.

### Exemples

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

### Voir aussi

* enum [SaveFormat](../../saveformat/)
* class [FileFormatUtil](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



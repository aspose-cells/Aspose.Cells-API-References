---
title: "FileFormatUtil.ExtensionToSaveFormat"
second_title: "Aspose.Cells för .NET API‑referens"
description: "FileFormatUtil‑metod. Konverterar en filnamnsändelse till ett SaveFormat‑värde"
type: docs
url: /sv/net/aspose.cells/fileformatutil/extensiontosaveformat/
---
## FileFormatUtil.ExtensionToSaveFormat method

Konverterar en filnamnsändelse till ett SaveFormat‑värde.

```csharp
public static SaveFormat ExtensionToSaveFormat(string extension)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| filändelse | String | Filändelsen. Kan vara med eller utan inledande punkt. Skiftlägesokänslig. |

### Anmärkningar

Om ändelsen inte kan kännas igen returneras Unknown.

### Exempel

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

### Se även

* enum [SaveFormat](../../saveformat/)
* class [FileFormatUtil](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



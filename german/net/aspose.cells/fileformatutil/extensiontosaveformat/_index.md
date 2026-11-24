---
title: "FileFormatUtil.ExtensionToSaveFormat"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "FileFormatUtil-Methode. Konvertiert eine Dateinamenerweiterung in einen SaveFormat-Wert"
type: docs
url: /de/net/aspose.cells/fileformatutil/extensiontosaveformat/
---
## FileFormatUtil.ExtensionToSaveFormat method

Konvertiert eine Dateinamenerweiterung in einen SaveFormat-Wert.

```csharp
public static SaveFormat ExtensionToSaveFormat(string extension)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Erweiterung | String | Die Dateierweiterung. Kann mit oder ohne führenden Punkt angegeben werden. Groß-/Kleinschreibung wird ignoriert. |

### Hinweise

Wenn die Erweiterung nicht erkannt wird, wird Unknown zurückgegeben.

### Beispiele

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

### Siehe auch

* enum [SaveFormat](../../saveformat/)
* class [FileFormatUtil](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



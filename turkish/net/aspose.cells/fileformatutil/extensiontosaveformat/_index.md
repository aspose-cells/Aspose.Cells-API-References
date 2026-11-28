---
title: "FileFormatUtil.ExtensionToSaveFormat"
second_title: "Aspose.Cells için .NET API Referansı"
description: "FileFormatUtil yöntemi. Bir dosya adı uzantısını SaveFormat değerine dönüştürür"
type: docs
url: /tr/net/aspose.cells/fileformatutil/extensiontosaveformat/
---
## FileFormatUtil.ExtensionToSaveFormat method

Bir dosya adı uzantısını SaveFormat değerine dönüştürür.

```csharp
public static SaveFormat ExtensionToSaveFormat(string extension)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| uzantı | String | Dosya uzantısı. Başında nokta olup olmadan olabilir. Büyük/küçük harfe duyarsız. |

### Açıklamalar

Uzantı tanınamazsa, Unknown döndürür.

### Örnekler

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

### Ayrıca Bakınız

* enum [SaveFormat](../../saveformat/)
* class [FileFormatUtil](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



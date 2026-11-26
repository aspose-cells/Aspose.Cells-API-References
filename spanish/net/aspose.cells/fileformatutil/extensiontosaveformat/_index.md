---
title: "FileFormatUtil.ExtensionToSaveFormat"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método FileFormatUtil. Convierte la extensión de un nombre de archivo en un valor SaveFormat"
type: docs
url: /es/net/aspose.cells/fileformatutil/extensiontosaveformat/
---
## FileFormatUtil.ExtensionToSaveFormat method

Convierte la extensión del nombre de archivo en un valor SaveFormat.

```csharp
public static SaveFormat ExtensionToSaveFormat(string extension)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| extensión | String | La extensión del archivo. Puede estar con o sin un punto inicial. No distingue mayúsculas y minúsculas. |

### Observaciones

Si la extensión no puede ser reconocida, devuelve Unknown.

### Ejemplos

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

### Ver también

* enum [SaveFormat](../../saveformat/)
* class [FileFormatUtil](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



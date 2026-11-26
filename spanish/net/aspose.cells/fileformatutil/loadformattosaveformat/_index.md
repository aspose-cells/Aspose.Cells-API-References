---
title: "FileFormatUtil.LoadFormatToSaveFormat"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método FileFormatUtil. Convierte un valor LoadFormat a un valor SaveFormat si es posible"
type: docs
url: /es/net/aspose.cells/fileformatutil/loadformattosaveformat/
---
## FileFormatUtil.LoadFormatToSaveFormat method

Convierte un valor LoadFormat a un valor SaveFormat si es posible.

```csharp
public static SaveFormat LoadFormatToSaveFormat(LoadFormat loadFormat)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| loadFormat | LoadFormat | El formato de carga. |

### Valor de retorno

El formato de guardado.

### Ejemplos

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

### Ver también

* enum [SaveFormat](../../saveformat/)
* enum [LoadFormat](../../loadformat/)
* class [FileFormatUtil](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



---
title: "FileFormatUtil.LoadFormatToSaveFormat"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод FileFormatUtil. Преобразует значение LoadFormat в значение SaveFormat, если это возможно."
type: docs
url: /ru/net/aspose.cells/fileformatutil/loadformattosaveformat/
---
## FileFormatUtil.LoadFormatToSaveFormat method

Преобразует значение LoadFormat в значение SaveFormat, если это возможно.

```csharp
public static SaveFormat LoadFormatToSaveFormat(LoadFormat loadFormat)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| loadFormat | LoadFormat | Формат загрузки. |

### Возвращаемое значение

Формат сохранения.

### Примеры

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

### См. также

* enum [SaveFormat](../../saveformat/)
* enum [LoadFormat](../../loadformat/)
* class [FileFormatUtil](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



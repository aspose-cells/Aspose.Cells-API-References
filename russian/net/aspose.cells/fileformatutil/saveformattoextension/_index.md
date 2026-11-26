---
title: "FileFormatUtil.SaveFormatToExtension"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод FileFormatUtil. Преобразует перечисленное значение формата сохранения в расширение файла."
type: docs
url: /ru/net/aspose.cells/fileformatutil/saveformattoextension/
---
## FileFormatUtil.SaveFormatToExtension method

Преобразует перечисленное значение формата сохранения в расширение файла.

```csharp
public static string SaveFormatToExtension(SaveFormat format)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| формат | SaveFormat | Формат сохранения. |

### Возвращаемое значение

Возвращаемое расширение — строка в нижнем регистре с ведущей точкой.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FileFormatUtilMethodSaveFormatToExtensionWithSaveFormatDemo
    {
        public static void Run()
        {
            // Создать пример рабочей книги
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test content");

            // Продемонстрировать SaveFormatToExtension с различными форматами.
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
                
                // Сохранить с обнаруженным расширением.
                string fileName = $"output{extension}";
                workbook.Save(fileName, options);
                Console.WriteLine($"Saved file: {fileName}");
            }

            workbook.Dispose();
        }
    }
}
```

### См. также

* enum [SaveFormat](../../saveformat/)
* class [FileFormatUtil](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



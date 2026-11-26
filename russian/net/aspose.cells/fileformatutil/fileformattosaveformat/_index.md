---
title: "FileFormatUtil.FileFormatToSaveFormat"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод FileFormatUtil. Преобразование формата файла в формат сохранения"
type: docs
url: /ru/net/aspose.cells/fileformatutil/fileformattosaveformat/
---
## FileFormatUtil.FileFormatToSaveFormat method

Преобразование формата файла в формат сохранения.

```csharp
public static SaveFormat FileFormatToSaveFormat(FileFormatType format)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| формат | FileFormatType | Тип формата файла. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FileFormatUtilMethodFileFormatToSaveFormatWithFileFormatTypeDemo
    {
        public static void Run()
        {
            // Создать пример рабочей книги
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test FileFormatToSaveFormat");

            // Получить тип формата файла рабочей книги
            FileFormatType originalFormat = workbook.FileFormat;

            // Преобразовать FileFormatType в SaveFormat
            SaveFormat saveFormat = FileFormatUtil.FileFormatToSaveFormat(originalFormat);

            // Сохранить рабочую книгу, используя преобразованный SaveFormat
            string outputPath = "Output_" + saveFormat.ToString() + ".xlsx";
            workbook.Save(outputPath, saveFormat);

            Console.WriteLine("File saved successfully with SaveFormat: " + saveFormat);
        }
    }
}
```

### См. также

* enum [SaveFormat](../../saveformat/)
* enum [FileFormatType](../../fileformattype/)
* class [FileFormatUtil](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



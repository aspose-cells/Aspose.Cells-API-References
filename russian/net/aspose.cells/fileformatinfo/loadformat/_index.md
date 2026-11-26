---
title: "FileFormatInfo.LoadFormat"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство FileFormatInfo. Возвращает обнаруженный формат загрузки"
type: docs
url: /ru/net/aspose.cells/fileformatinfo/loadformat/
---
## FileFormatInfo.LoadFormat property

Получает обнаруженный формат загрузки.

```csharp
public LoadFormat LoadFormat { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FileFormatInfoPropertyLoadFormatDemo
    {
        public static void Run()
        {
            // Путь к каталогу документов.
            string filePath = "data/";
            
            // Определить формат файла
            string fileName = "SAMPLE_XLS_ISSUE.XLS";
            var fileFormatInfo = FileFormatUtil.DetectFileFormat(filePath + fileName);
            Console.WriteLine("Detected LoadFormat: " + fileFormatInfo.LoadFormat);

            // Загрузить файл с правильным форматом
            LoadOptions loadOptions = new LoadOptions(LoadFormat.MHtml);
            var workbook = new Workbook(filePath + fileName, loadOptions);
            
            // Обработать книгу
            workbook.Worksheets[0].AutoFitColumns();
            workbook.Save(filePath + "output.xlsx");
        }
    }
}
```

### См. также

* enum [LoadFormat](../../loadformat/)
* class [FileFormatInfo](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



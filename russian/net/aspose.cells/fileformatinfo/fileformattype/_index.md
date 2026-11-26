---
title: "FileFormatInfo.FileFormatType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство FileFormatInfo. Возвращает обнаруженный формат файла"
type: docs
url: /ru/net/aspose.cells/fileformatinfo/fileformattype/
---
## FileFormatInfo.FileFormatType property

Получает обнаруженный формат файла.

```csharp
public FileFormatType FileFormatType { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FileFormatInfoPropertyFileFormatTypeDemo
    {
        public static void Run()
        {
            // Пример 1: Обнаружить формат Excel 97-2003
            string excelFile = "sample.xls";
            FileFormatInfo info = FileFormatUtil.DetectFileFormat(excelFile);
            Console.WriteLine("File Format Type: " + info.FileFormatType);
            Console.WriteLine("Is Encrypted: " + info.IsEncrypted);

            // Пример 2: Обнаружить формат OOXML
            string xlsxFile = "sample.xlsx";
            info = FileFormatUtil.DetectFileFormat(xlsxFile);
            Console.WriteLine("File Format Type: " + info.FileFormatType);
            Console.WriteLine("Is Encrypted: " + info.IsEncrypted);
        }
    }
}
```

### См. также

* enum [FileFormatType](../../fileformattype/)
* class [FileFormatInfo](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



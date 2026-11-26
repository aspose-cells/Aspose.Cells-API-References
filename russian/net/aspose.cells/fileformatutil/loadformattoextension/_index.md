---
title: "FileFormatUtil.LoadFormatToExtension"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод FileFormatUtil. Преобразует перечисленное значение формата загрузки в расширение файла."
type: docs
url: /ru/net/aspose.cells/fileformatutil/loadformattoextension/
---
## FileFormatUtil.LoadFormatToExtension method

Преобразует перечисленное значение формата загрузки в расширение файла.

```csharp
public static string LoadFormatToExtension(LoadFormat loadFormat)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| loadFormat | LoadFormat | Загруженный формат файла. |

### Возвращаемое значение

Возвращаемое расширение — строка в нижнем регистре с ведущей точкой.

### Примечания

Если не может быть преобразовано, возвращает null.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FileFormatUtilMethodLoadFormatToExtensionWithLoadFormatDemo
    {
        public static void Run()
        {
            // Продемонстрировать LoadFormatToExtension с различными значениями LoadFormat
            Console.WriteLine("Auto format extension: " + FileFormatUtil.LoadFormatToExtension(LoadFormat.Auto));
            Console.WriteLine("CSV format extension: " + FileFormatUtil.LoadFormatToExtension(LoadFormat.Csv));
            Console.WriteLine("Excel97-2003 format extension: " + FileFormatUtil.LoadFormatToExtension(LoadFormat.Excel97To2003));
            Console.WriteLine("XLSX format extension: " + FileFormatUtil.LoadFormatToExtension(LoadFormat.Xlsx));
            Console.WriteLine("TSV format extension: " + FileFormatUtil.LoadFormatToExtension(LoadFormat.Tsv));
            Console.WriteLine("ODS format extension: " + FileFormatUtil.LoadFormatToExtension(LoadFormat.Ods));
            Console.WriteLine("XLSB format extension: " + FileFormatUtil.LoadFormatToExtension(LoadFormat.Xlsb));
        }
    }
}
```

### См. также

* enum [LoadFormat](../../loadformat/)
* class [FileFormatUtil](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



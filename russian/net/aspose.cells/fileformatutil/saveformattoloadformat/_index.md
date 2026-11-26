---
title: "FileFormatUtil.SaveFormatToLoadFormat"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод FileFormatUtil. Преобразует значение SaveFormat в значение LoadFormat, если это возможно"
type: docs
url: /ru/net/aspose.cells/fileformatutil/saveformattoloadformat/
---
## FileFormatUtil.SaveFormatToLoadFormat method

Преобразует значение SaveFormat в значение LoadFormat, если это возможно.

```csharp
public static LoadFormat SaveFormatToLoadFormat(SaveFormat saveFormat)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| saveFormat | SaveFormat | Формат сохранения. |

### Возвращаемое значение

Формат загрузки

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FileFormatUtilMethodSaveFormatToLoadFormatWithSaveFormatDemo
    {
        public static void Run()
        {
            // Продемонстрировать преобразования SaveFormatToLoadFormat
            Console.WriteLine("SaveFormat to LoadFormat Conversion Examples:");
            
            LoadFormat excel97To2003 = FileFormatUtil.SaveFormatToLoadFormat(SaveFormat.Excel97To2003);
            Console.WriteLine($"SaveFormat.Excel97To2003 -> {excel97To2003}");

            LoadFormat xlsx = FileFormatUtil.SaveFormatToLoadFormat(SaveFormat.Xlsx);
            Console.WriteLine($"SaveFormat.Xlsx -> {xlsx}");

            LoadFormat tsv = FileFormatUtil.SaveFormatToLoadFormat(SaveFormat.Tsv);
            Console.WriteLine($"SaveFormat.Tsv -> {tsv}");

            LoadFormat ods = FileFormatUtil.SaveFormatToLoadFormat(SaveFormat.Ods);
            Console.WriteLine($"SaveFormat.Ods -> {ods}");

            LoadFormat xlsb = FileFormatUtil.SaveFormatToLoadFormat(SaveFormat.Xlsb);
            Console.WriteLine($"SaveFormat.Xlsb -> {xlsb}");
        }
    }
}
```

### См. также

* enum [LoadFormat](../../loadformat/)
* enum [SaveFormat](../../saveformat/)
* class [FileFormatUtil](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



---
title: "TxtLoadOptions.Separator"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство TxtLoadOptions. Получает и задает символ-разделитель текстового файла"
type: docs
url: /ru/net/aspose.cells/txtloadoptions/separator/
---
## TxtLoadOptions.Separator property

Получает и задаёт символьный разделитель текстового файла.

```csharp
public char Separator { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtLoadOptionsPropertySeparatorDemo
    {
        public static void Run()
        {
            // Создайте примерные данные и сохраните их с пользовательским разделителем
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);

            TxtSaveOptions saveOptions = new TxtSaveOptions();
            saveOptions.Separator = '*';
            workbook.Save("output.csv", saveOptions);

            // Загрузите сохранённый файл с тем же разделителем
            TxtLoadOptions loadOptions = new TxtLoadOptions();
            loadOptions.Separator = '*';
            Workbook loadedWorkbook = new Workbook("output.csv", loadOptions);

            // Проверьте загруженные данные
            Worksheet loadedSheet = loadedWorkbook.Worksheets[0];
            Console.WriteLine("A1: " + loadedSheet.Cells["A1"].StringValue);
            Console.WriteLine("B1: " + loadedSheet.Cells["B1"].StringValue);
        }
    }
}
```

### См. также

* class [TxtLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



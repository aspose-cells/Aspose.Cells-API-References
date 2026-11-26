---
title: "TxtSaveOptions.SeparatorString"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство TxtSaveOptions. Получает и задает строковое значение в качестве разделителя"
type: docs
url: /ru/net/aspose.cells/txtsaveoptions/separatorstring/
---
## TxtSaveOptions.SeparatorString property

Получает и задаёт строковое значение в качестве разделителя.

```csharp
public string SeparatorString { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtSaveOptionsPropertySeparatorStringDemo
    {
        public static void Run()
        {
            // Создать пример рабочей книги с тестовыми данными
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить тестовые данные
            worksheet.Cells["A1"].PutValue("Column1");
            worksheet.Cells["B1"].PutValue("Column2");
            worksheet.Cells["A2"].PutValue("Data1");
            worksheet.Cells["B2"].PutValue("Data2");
            worksheet.Cells["A3"].PutValue(1);
            worksheet.Cells["B3"].PutValue(2);

            // Сохранить с разделителем пробел
            TxtSaveOptions saveOptions = new TxtSaveOptions();
            saveOptions.SeparatorString = " ";
            workbook.Save("output_space.txt", saveOptions);

            // Сохранить с разделителем «|»
            saveOptions.SeparatorString = "|";
            workbook.Save("output_pipe.txt", saveOptions);

            // Загрузите файл с разделителями пробелами для проверки
            TxtLoadOptions loadOptions = new TxtLoadOptions();
            loadOptions.SeparatorString = " ";
            Workbook loadedWorkbook = new Workbook("output_space.txt", loadOptions);
            Cells cells = loadedWorkbook.Worksheets[0].Cells;

            Console.WriteLine("Space-separated values:");
            Console.WriteLine($"{cells["A1"].StringValue} {cells["B1"].StringValue}");
            Console.WriteLine($"{cells["A2"].StringValue} {cells["B2"].StringValue}");
            Console.WriteLine($"{cells["A3"].IntValue} {cells["B3"].IntValue}");
        }
    }
}
```

### См. также

* class [TxtSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



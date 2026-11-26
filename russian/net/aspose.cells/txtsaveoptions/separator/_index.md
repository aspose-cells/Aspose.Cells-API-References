---
title: "TxtSaveOptions.Separator"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство TxtSaveOptions. Получает и задает символ-разделитель текстового файла"
type: docs
url: /ru/net/aspose.cells/txtsaveoptions/separator/
---
## TxtSaveOptions.Separator property

Получает и задает символ-разделитель текстового файла.

```csharp
public char Separator { get; set; }
```

### Примеры

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtSaveOptionsPropertySeparatorDemo
    {
        public static void Run()
        {
            // Создать пример рабочей книги с тестовыми данными
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // Настройте параметры сохранения TXT с запятой в качестве разделителя
            TxtSaveOptions txtSaveOptions = new TxtSaveOptions();
            txtSaveOptions.Separator = ',';
            txtSaveOptions.Encoding = System.Text.Encoding.UTF8;

            // Сохранить книгу как CSV с запятой в качестве разделителя
            string outputPath = "output.csv";
            workbook.Save(outputPath, txtSaveOptions);

            // Отобразить содержимое сохранённого файла
            Console.WriteLine("File saved with comma separator:");
            Console.WriteLine(File.ReadAllText(outputPath));
        }
    }
}
```

### См. также

* class [TxtSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



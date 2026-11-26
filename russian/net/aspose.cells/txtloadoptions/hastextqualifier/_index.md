---
title: "TxtLoadOptions.HasTextQualifier"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство TxtLoadOptions. Указывает, есть ли текстовый квалификатор для значения ячейки. По умолчанию true"
type: docs
url: /ru/net/aspose.cells/txtloadoptions/hastextqualifier/
---
## TxtLoadOptions.HasTextQualifier property

Определяет, есть ли текстовый квалификатор для значения ячейки. По умолчанию true.

```csharp
public bool HasTextQualifier { get; set; }
```

### Примеры

```csharp
using System;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtLoadOptionsPropertyHasTextQualifierDemo
    {
        public static void Run()
        {
            // Создайте содержимое CSV с текстовыми квалификаторами
            string csvContent = "\"Name\",\"Age\",\"City\"\n\"John\",30,\"New York\"\n\"Alice\",25,\"London\"";
            
            // Сохраните содержимое CSV во временный файл
            string tempFile = "temp.csv";
            System.IO.File.WriteAllText(tempFile, csvContent, Encoding.UTF8);

            // Создайте TxtLoadOptions с HasTextQualifier, установленным в true
            TxtLoadOptions loadOptions = new TxtLoadOptions(LoadFormat.Csv)
            {
                Separator = ',',
                HasTextQualifier = true,
                TextQualifier = '\"'
            };

            // Загрузите файл CSV с текстовыми квалификаторами
            Workbook workbook = new Workbook(tempFile, loadOptions);

            // Сохраните книгу, чтобы продемонстрировать успешную загрузку
            workbook.Save("Output.xlsx");

            // Очистите временный файл
            System.IO.File.Delete(tempFile);
        }
    }
}
```

### См. также

* class [TxtLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



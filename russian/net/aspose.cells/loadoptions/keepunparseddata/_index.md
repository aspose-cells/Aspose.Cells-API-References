---
title: "LoadOptions.KeepUnparsedData"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство LoadOptions. Указывает, сохранять ли неразобранные данные в памяти для Workbook при загрузке из файла шаблона. Значение по умолчанию — true"
type: docs
url: /ru/net/aspose.cells/loadoptions/keepunparseddata/
---
## LoadOptions.KeepUnparsedData property

Определяет, сохранять ли неразобранные данные в памяти для Workbook при загрузке из шаблонного файла. По умолчанию true.

```csharp
public bool KeepUnparsedData { get; set; }
```

### Примечания

Для сценариев, когда пользователю нужно только читать некоторые содержимые из шаблонного файла и не требуется сохранять книгу обратно, установка этого свойства в false может улучшить производительность, особенно при совместном использовании с некоторыми типами LoadFilter,

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyKeepUnparsedDataDemo
    {
        public static void Run()
        {
            // Создайте параметры загрузки и установите KeepUnparsedData в false
            LoadOptions options = new LoadOptions();
            options.KeepUnparsedData = false;

            // Загрузить книгу с параметрами
            Workbook workbook = new Workbook("example.xlsx", options);

            // Получите доступ к листу и продемонстрируйте, что неразобранные данные не сохраняются
            Worksheet worksheet = workbook.Worksheets[0];
            Console.WriteLine("Cell A1 value: " + worksheet.Cells["A1"].Value);

            // Сохраните книгу
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



---
title: "ExternalLink.Type"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ExternalLink. Возвращает тип внешней ссылки"
type: docs
url: /ru/net/aspose.cells/externallink/type/
---
## ExternalLink.Type property

Получает тип внешней ссылки.

```csharp
public ExternalLinkType Type { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExternalLinkPropertyTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Добавить лист
            Worksheet sheet = workbook.Worksheets[0];
            
            // Создайте внешнюю ссылку на другую книгу
            sheet.Cells["A1"].Formula = "='[link.xls]Sheet1'!A1";
            
            // Получить внешнюю ссылку
            ExternalLink externalLink = workbook.Worksheets.ExternalLinks[0];
            
            // Отобразить тип внешней ссылки
            Console.WriteLine("External Link Type: " + externalLink.Type);
            
            // Изменить источник данных внешней ссылки
            externalLink.DataSource = "d:\\link.xls";
            
            // Сохраните книгу
            workbook.Save("ExternalLinkTypeExample.xlsx");
        }
    }
}
```

### См. также

* enum [ExternalLinkType](../../externallinktype/)
* class [ExternalLink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



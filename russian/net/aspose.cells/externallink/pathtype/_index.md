---
title: "ExternalLink.PathType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ExternalLink. Получить тип пути этой внешней ссылки"
type: docs
url: /ru/net/aspose.cells/externallink/pathtype/
---
## ExternalLink.PathType property

Получить тип пути этой внешней ссылки

```csharp
public string PathType { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExternalLinkPropertyPathTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Добавить лист
            Worksheet sheet = workbook.Worksheets[0];
            
            // Создайте внешнюю ссылку на другую книгу
            sheet.Cells["A1"].Formula = "='C:\\Temp\\ExternalWorkbook.xlsx'!Sheet1!A1";
            
            // Получить внешнюю ссылку
            ExternalLink externalLink = workbook.Worksheets.ExternalLinks[0];
            
            // Отобразите тип пути внешней ссылки
            Console.WriteLine("Path Type: " + externalLink.PathType);
            
            // Сохраните книгу
            workbook.Save("ExternalLinkDemo.xlsx");
        }
    }
}
```

### См. также

* class [ExternalLink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



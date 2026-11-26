---
title: "Worksheet.Hyperlinks"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Worksheet. Получает коллекцию HyperlinkCollection"
type: docs
url: /ru/net/aspose.cells/worksheet/hyperlinks/
---
## Worksheet.Hyperlinks property

Получает коллекцию [`HyperlinkCollection`](../../hyperlinkcollection/).

```csharp
public HyperlinkCollection Hyperlinks { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyHyperlinksDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте гиперссылку в лист
            worksheet.Hyperlinks.Add(0, 0, 1, 1, @"https://www.aspose.com");
            
            // Сохраните книгу
            workbook.Save("HyperlinksDemo.xlsx");
            
            // Загрузите сохранённую книгу, чтобы проверить гиперссылку
            Workbook loadedWorkbook = new Workbook("HyperlinksDemo.xlsx");
            Worksheet loadedWorksheet = loadedWorkbook.Worksheets[0];
            
            // Отобразить адрес гиперссылки
            Console.WriteLine("Hyperlink Address: " + loadedWorksheet.Hyperlinks[0].Address);
        }
    }
}
```

### См. также

* class [HyperlinkCollection](../../hyperlinkcollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



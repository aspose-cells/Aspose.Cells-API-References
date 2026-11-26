---
title: "FindOptions.SearchNext"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство FindOptions. Порядок поиска. True — искать следующий. False — искать предыдущий"
type: docs
url: /ru/net/aspose.cells/findoptions/searchnext/
---
## FindOptions.SearchNext property

Порядок поиска. True: искать следующий. False: искать предыдущий.

```csharp
[Obsolete("Use FindOptions.SearchBackward property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool SearchNext { get; set; }
```

### Примечания

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него используйте свойство FindOptions.SearchBackward. Это свойство будет удалено через 12 месяцев, начиная с ноября 2018 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FindOptionsPropertySearchNextDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Заполните некоторыми образцовыми данными
            worksheet.Cells["A1"].PutValue("Apple");
            worksheet.Cells["A2"].PutValue("Banana");
            worksheet.Cells["A3"].PutValue("apple");
            worksheet.Cells["A4"].PutValue("Orange");
            worksheet.Cells["A5"].PutValue("apple pie");

            // Создайте параметры поиска
            FindOptions findOptions = new FindOptions();
            findOptions.CaseSensitive = false;
            findOptions.LookAtType = LookAtType.Contains;

            // Продемонстрировать свойство SearchNext (устарело, но показано для демонстрации)
            Console.WriteLine("Initial SearchNext value: " + findOptions.SearchNext);
            
            // Поиск вперёд (поведение по умолчанию)
            findOptions.SearchNext = true;
            Cell firstForward = worksheet.Cells.Find("apple", null, findOptions);
            Console.WriteLine("First forward search result: " + (firstForward != null ? firstForward.Name + " - " + firstForward.StringValue : "Not found"));

            // Поиск назад
            findOptions.SearchNext = false;
            Cell firstBackward = worksheet.Cells.Find("apple", null, findOptions);
            Console.WriteLine("First backward search result: " + (firstBackward != null ? firstBackward.Name + " - " + firstBackward.StringValue : "Not found"));

            // Сохраните книгу
            workbook.Save("PropertySearchNextDemo.xlsx");
        }
    }
}
```

### См. также

* class [FindOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



---
title: "Класс SmartTagSetting"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Aspose.Cells.Markup.SmartTagSetting class. Представляет все объекты SmartTagCollection в листе"
type: docs
url: /ru/net/aspose.cells.markup/smarttagsetting/
---
## SmartTagSetting class

Представляет все объекты [`SmartTagCollection`](../smarttagcollection/) в листе.

```csharp
public class SmartTagSetting : CollectionBase
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Item](../../aspose.cells.markup/smarttagsetting/item/) { get; } | Получает объект [`SmartTagCollection`](../smarttagcollection/) по индексу. (3 индексатора) |

## Методы

| Имя | Описание |
| --- | --- |
| [Add](../../aspose.cells.markup/smarttagsetting/add/#add_1)(string) | Добавить смарт‑теги ячейки. |
| [Add](../../aspose.cells.markup/smarttagsetting/add/#add)(int, int) | Добавляет объект [`SmartTagCollection`](../smarttagcollection/) в ячейку. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Markup;
    using System;

    public class SmartTagSettingDemo
    {
        public static void SmartTagSettingExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить смарт‑тег в конкретную ячейку
            SmartTagSetting smartTagSetting = worksheet.SmartTagSetting;
            int smartTagIndex = smartTagSetting.Add(0, 0); // Adding smart tag to cell A1

            // Получить доступ к SmartTagCollection для ячейки
            SmartTagCollection smartTagCollection = smartTagSetting[0, 0];

            // Добавить смарт‑тег в коллекцию
            int tagIndex = smartTagCollection.Add("urn:schemas-microsoft-com:office:smarttags", "date");

            // Установить ёмкость настройки смарт‑тега
            smartTagSetting.Capacity = 10;

            // Вывести количество смарт‑тегов
            Console.WriteLine("Total Smart Tags: " + smartTagSetting.Count);

            // Сохраните книгу
            workbook.Save("SmartTagSettingExample.xlsx");

            return;
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Markup](../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../)



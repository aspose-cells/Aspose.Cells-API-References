---
title: "Перечисление UpdateLinksType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.UpdateLinksType. Представляет, как обновлять ссылки на другие книги при открытии книги"
type: docs
url: /ru/net/aspose.cells/updatelinkstype/
---
## UpdateLinksType enumeration

Представляет, как обновлять ссылки на другие книги при открытии книги.

```csharp
public enum UpdateLinksType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| UserSet | `0` | Запросить у пользователя обновление. |
| Never | `1` | Не обновлять и не запрашивать у пользователя. |
| Always | `2` | Всегда обновлять. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class UpdateLinksTypeDemo
    {
        public static void UpdateLinksTypeExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Получить доступ к настройкам книги
            WorkbookSettings settings = workbook.Settings;

            // Установить UpdateLinksType в значение Always update
            settings.UpdateLinksType = UpdateLinksType.Always;

            // Добавить новый лист в книгу
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные в лист
            worksheet.Cells["A1"].PutValue("External Link Example");
            worksheet.Cells["A2"].PutValue("Data");

            // Сохраните книгу
            workbook.Save("UpdateLinksTypeExample.xlsx");

            // Вывести текущую настройку UpdateLinksType
            Console.WriteLine("UpdateLinksType is set to: " + settings.UpdateLinksType);
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)



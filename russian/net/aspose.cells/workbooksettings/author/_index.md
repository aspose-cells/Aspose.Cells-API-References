---
title: "WorkbookSettings.Author"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство WorkbookSettings. Получает и задает автора файла"
type: docs
url: /ru/net/aspose.cells/workbooksettings/author/
---
## WorkbookSettings.Author property

Получает и задаёт автора файла.

```csharp
public string Author { get; set; }
```

### Примечания

Не установлено, сначала проверьте [`Author`](../../../aspose.cells.properties/builtindocumentpropertycollection/author/), затем проверьте пользователя Environment.

### Примеры

```csharp
using System;
using System.Globalization;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyAuthorDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Доступ к WorkbookSettings
            WorkbookSettings settings = workbook.Settings;

            // Установить свойство автора
            settings.Author = "John Doe";

            // Добавьте некоторые примерные данные, чтобы продемонстрировать функциональность книги
            Worksheet sheet = workbook.Worksheets[0];
            sheet.Cells["A1"].PutValue("Sample Workbook");
            sheet.Cells["A2"].PutValue("Created by: " + settings.Author);
            sheet.Cells["A3"].PutValue(DateTime.Now.ToString());

            // Сохраните книгу
            workbook.Save("AuthorDemo.xlsx");
        }
    }
}
```

### См. также

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



---
title: "WorkbookSettings.Shared"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство WorkbookSettings. Получает или задает значение, указывающее, является ли книга общей"
type: docs
url: /ru/net/aspose.cells/workbooksettings/shared/
---
## WorkbookSettings.Shared property

Получает или задает значение, указывающее, является ли книга общей.

```csharp
public bool Shared { get; set; }
```

### Примечания

Значение по умолчанию — false.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertySharedDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook book = new Workbook();
            
            // Установите свойство Shared в значение true
            book.Settings.Shared = true;
            
            // Сохраните книгу
            string outputPath = "output_shared.xlsx";
            book.Save(outputPath);
            
            // Загрузите сохранённую книгу, чтобы проверить свойство Shared
            Workbook loadedBook = new Workbook(outputPath);
            Console.WriteLine("Shared property value: " + loadedBook.Settings.Shared);
        }
    }
}
```

### См. также

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



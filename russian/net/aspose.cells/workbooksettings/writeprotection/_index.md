---
title: "WorkbookSettings.WriteProtection"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство WorkbookSettings. Предоставляет доступ к параметрам защиты записи книги"
type: docs
url: /ru/net/aspose.cells/workbooksettings/writeprotection/
---
## WorkbookSettings.WriteProtection property

Предоставляет доступ к параметрам защиты книги от записи.

```csharp
public WriteProtection WriteProtection { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyWriteProtectionDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Установить свойства защиты записи
            workbook.Settings.WriteProtection.Password = "test123";
            workbook.Settings.WriteProtection.Author = "John Doe";
            workbook.Settings.WriteProtection.RecommendReadOnly = true;

            // Сохраните книгу
            string outputPath = "WriteProtectionDemo.xlsx";
            workbook.Save(outputPath);

            // Загрузите сохранённую книгу, чтобы проверить свойства
            Workbook loadedWorkbook = new Workbook(outputPath);
            
            // Вывести свойства защиты записи
            Console.WriteLine("Author: " + loadedWorkbook.Settings.WriteProtection.Author);
            Console.WriteLine("ReadOnly Recommended: " + loadedWorkbook.Settings.WriteProtection.RecommendReadOnly);
        }
    }
}
```

### См. также

* class [WriteProtection](../../writeprotection/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



---
title: "WorkbookSettings.UpdateLinksType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство WorkbookSettings. Получает и задает, как обновлять внешние ссылки при открытии книги"
type: docs
url: /ru/net/aspose.cells/workbooksettings/updatelinkstype/
---
## WorkbookSettings.UpdateLinksType property

Получает и задает, как обновлять внешние ссылки при открытии книги.

```csharp
public UpdateLinksType UpdateLinksType { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyUpdateLinksTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Установите UpdateLinksType в Never
            workbook.Settings.UpdateLinksType = UpdateLinksType.Never;
            
            // Сохраните книгу
            workbook.Save("output.xlsx");
            
            // Загрузите сохранённую книгу, чтобы проверить настройку
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            
            // Выведите значение UpdateLinksType
            Console.WriteLine("UpdateLinksType: " + loadedWorkbook.Settings.UpdateLinksType);
        }
    }
}
```

### См. также

* enum [UpdateLinksType](../../updatelinkstype/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



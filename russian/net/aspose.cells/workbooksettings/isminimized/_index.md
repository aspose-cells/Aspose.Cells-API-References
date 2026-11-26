---
title: "WorkbookSettings.IsMinimized"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство WorkbookSettings. Представляет, будет ли сгенерированная таблица открыта в свернутом виде"
type: docs
url: /ru/net/aspose.cells/workbooksettings/isminimized/
---
## WorkbookSettings.IsMinimized property

Отражает, будет ли сгенерированная таблица открыта в свернутом виде.

```csharp
public bool IsMinimized { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyIsMinimizedDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Установите свойство IsMinimized в true
            workbook.Settings.IsMinimized = true;

            // Сохраните книгу
            workbook.Save("IsMinimizedDemo.xlsx");

            // Загрузить сохранённую книгу, чтобы проверить свойство
            Workbook loadedWorkbook = new Workbook("IsMinimizedDemo.xlsx");

            // Выведите значение свойства IsMinimized
            Console.WriteLine("Workbook IsMinimized property: " + loadedWorkbook.Settings.IsMinimized);
        }
    }
}
```

### См. также

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



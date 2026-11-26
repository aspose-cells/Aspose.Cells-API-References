---
title: "WorkbookSettings.IsHidden"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство WorkbookSettings. Указывает, скрыта ли эта рабочая книга"
type: docs
url: /ru/net/aspose.cells/workbooksettings/ishidden/
---
## WorkbookSettings.IsHidden property

Указывает, скрыта ли эта рабочая книга.

```csharp
public bool IsHidden { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyIsHiddenDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Доступ к настройкам рабочей книги
            WorkbookSettings settings = workbook.Settings;

            // Установите свойство IsHidden в значение true
            settings.IsHidden = true;
            Console.WriteLine("Workbook is hidden: " + settings.IsHidden);

            // Сохраните книгу
            workbook.Save("WorkbookSettings_IsHidden_True.xlsx");

            // Создайте другую рабочую книгу
            Workbook workbook2 = new Workbook();

            // Доступ к настройкам рабочей книги
            WorkbookSettings settings2 = workbook2.Settings;

            // Установите свойство IsHidden в значение false (по умолчанию)
            settings2.IsHidden = false;
            Console.WriteLine("Workbook is hidden: " + settings2.IsHidden);

            // Сохраните книгу
            workbook2.Save("WorkbookSettings_IsHidden_False.xlsx");

            // Загрузите и проверьте сохранённые рабочие книги
            Workbook loadedWorkbook1 = new Workbook("WorkbookSettings_IsHidden_True.xlsx");
            Console.WriteLine("Loaded workbook1 is hidden: " + loadedWorkbook1.Settings.IsHidden);

            Workbook loadedWorkbook2 = new Workbook("WorkbookSettings_IsHidden_False.xlsx");
            Console.WriteLine("Loaded workbook2 is hidden: " + loadedWorkbook2.Settings.IsHidden);
        }
    }
}
```

### См. также

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



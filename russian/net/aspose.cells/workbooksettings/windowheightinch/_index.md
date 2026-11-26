---
title: "WorkbookSettings.WindowHeightInch"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство WorkbookSettings. Высота окна в дюймах"
type: docs
url: /ru/net/aspose.cells/workbooksettings/windowheightinch/
---
## WorkbookSettings.WindowHeightInch property

Высота окна в дюймах.

```csharp
public double WindowHeightInch { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyWindowHeightInchDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Доступ к настройкам рабочей книги
            WorkbookSettings settings = workbook.Settings;

            // Установить высоту окна в дюймах
            settings.WindowHeightInch = 5.5;

            // Отобразить высоту окна в дюймах
            Console.WriteLine("Window Height in Inches: " + settings.WindowHeightInch);

            // Сохраните книгу
            workbook.Save("WindowHeightInchDemo.xlsx");
        }
    }
}
```

### См. также

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



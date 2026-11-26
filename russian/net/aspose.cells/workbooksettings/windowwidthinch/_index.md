---
title: "WorkbookSettings.WindowWidthInch"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство WorkbookSettings. Ширина окна в дюймах"
type: docs
url: /ru/net/aspose.cells/workbooksettings/windowwidthinch/
---
## WorkbookSettings.WindowWidthInch property

Ширина окна в дюймах.

```csharp
public double WindowWidthInch { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyWindowWidthInchDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Доступ к настройкам рабочей книги
            WorkbookSettings settings = workbook.Settings;

            // Установить ширину окна в дюймах
            settings.WindowWidthInch = 10.5;

            // Отобразить ширину окна в дюймах
            Console.WriteLine("Window Width in Inches: " + settings.WindowWidthInch);

            // Сохраните книгу
            workbook.Save("WindowWidthInchDemo.xlsx");
        }
    }
}
```

### См. также

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



---
title: "WorkbookSettings.WindowTopInch"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство WorkbookSettings. Расстояние от верхнего края клиентской области до верхнего края окна в дюймах"
type: docs
url: /ru/net/aspose.cells/workbooksettings/windowtopinch/
---
## WorkbookSettings.WindowTopInch property

Расстояние от верхнего края клиентской области до верхнего края окна в дюймах.

```csharp
public double WindowTopInch { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyWindowTopInchDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Доступ к WorkbookSettings
            WorkbookSettings settings = workbook.Settings;

            // Установите свойство WindowTopInch, чтобы разместить окно на расстоянии 2 дюйма от верха
            settings.WindowTopInch = 2.0;

            // Проверьте настройку, распечатав её
            Console.WriteLine("Window top position (inches): " + settings.WindowTopInch);

            // Сохраните книгу
            workbook.Save("WindowTopInchDemo.xlsx");
        }
    }
}
```

### См. также

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



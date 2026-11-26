---
title: "WorkbookSettings.WindowTop"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство WorkbookSettings. Расстояние от верхнего края клиентской области до верхнего края окна в единицах пункта"
type: docs
url: /ru/net/aspose.cells/workbooksettings/windowtop/
---
## WorkbookSettings.WindowTop property

Расстояние от верхнего края клиентской области до верхнего края окна в пунктах.

```csharp
public double WindowTop { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyWindowTopDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Доступ к WorkbookSettings
            WorkbookSettings settings = workbook.Settings;

            // Установите свойство WindowTop, чтобы разместить окно на 100 пикселей от верха
            settings.WindowTop = 100;
            
            // Проверьте значение WindowTop
            Console.WriteLine("Window top position set to: " + settings.WindowTop);

            // Сохраните книгу
            workbook.Save("WindowTopDemo.xlsx");
        }
    }
}
```

### См. также

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



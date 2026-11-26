---
title: "WorkbookSettings.WindowWidth"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство WorkbookSettings. Ширина окна в единицах пункта"
type: docs
url: /ru/net/aspose.cells/workbooksettings/windowwidth/
---
## WorkbookSettings.WindowWidth property

Ширина окна в пунктах.

```csharp
public double WindowWidth { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyWindowWidthDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Доступ к WorkbookSettings
            WorkbookSettings settings = workbook.Settings;
            
            // Установить свойство WindowWidth
            settings.WindowWidth = 800;
            
            // Проверить значение WindowWidth
            Console.WriteLine("Window Width set to: " + settings.WindowWidth);
            
            // Сохраните книгу
            workbook.Save("WindowWidthDemo.xlsx");
        }
    }
}
```

### См. также

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



---
title: "WorkbookSettings.WindowHeight"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство WorkbookSettings. Высота окна в единицах точек"
type: docs
url: /ru/net/aspose.cells/workbooksettings/windowheight/
---
## WorkbookSettings.WindowHeight property

Высота окна в пунктах.

```csharp
public double WindowHeight { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyWindowHeightDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Доступ к WorkbookSettings
            WorkbookSettings settings = workbook.Settings;
            
            // Установите свойство WindowHeight
            settings.WindowHeight = 600;
            
            // Проверьте значение WindowHeight
            Console.WriteLine("Window Height set to: " + settings.WindowHeight);
            
            // Сохраните книгу
            workbook.Save("WindowHeightDemo.xlsx");
        }
    }
}
```

### См. также

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



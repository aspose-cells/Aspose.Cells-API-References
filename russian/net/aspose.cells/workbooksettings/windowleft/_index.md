---
title: "WorkbookSettings.WindowLeft"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство WorkbookSettings. Расстояние от левого края клиентской области до левого края окна в единицах пункта"
type: docs
url: /ru/net/aspose.cells/workbooksettings/windowleft/
---
## WorkbookSettings.WindowLeft property

Расстояние от левого края клиентской области до левого края окна в пунктах.

```csharp
public double WindowLeft { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyWindowLeftDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Доступ к WorkbookSettings
            WorkbookSettings settings = workbook.Settings;

            // Установите свойство WindowLeft, чтобы разместить окно на 100 пикселей от левого края
            settings.WindowLeft = 100;

            // Установите другие свойства окна для демонстрации
            settings.WindowTop = 50;
            settings.WindowWidth = 800;
            settings.WindowHeight = 600;

            // Добавить примерные данные в лист
            Worksheet sheet = workbook.Worksheets[0];
            sheet.Cells["A1"].PutValue("Window Position Demo");
            sheet.Cells["A2"].PutValue($"Left: {settings.WindowLeft}px");
            sheet.Cells["A3"].PutValue($"Top: {settings.WindowTop}px");

            // Сохраните книгу
            workbook.Save("WindowPositionDemo.xlsx");
        }
    }
}
```

### См. также

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



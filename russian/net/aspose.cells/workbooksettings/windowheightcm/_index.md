---
title: "WorkbookSettings.WindowHeightCM"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство WorkbookSettings. Высота окна в единицах сантиметров"
type: docs
url: /ru/net/aspose.cells/workbooksettings/windowheightcm/
---
## WorkbookSettings.WindowHeightCM property

Высота окна в сантиметрах.

```csharp
public double WindowHeightCM { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyWindowHeightCMDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Доступ к настройкам рабочей книги
            WorkbookSettings settings = workbook.Settings;

            // Установить свойство WindowHeightCM
            settings.WindowHeightCM = 15.5;

            // Отобразить установленное значение
            Console.WriteLine("Window Height in Centimeters: " + settings.WindowHeightCM);

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



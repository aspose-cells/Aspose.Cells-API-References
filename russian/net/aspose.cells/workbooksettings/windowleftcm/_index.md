---
title: "WorkbookSettings.WindowLeftCM"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство WorkbookSettings. Расстояние от левого края клиентской области до левого края окна. В единицах сантиметров"
type: docs
url: /ru/net/aspose.cells/workbooksettings/windowleftcm/
---
## WorkbookSettings.WindowLeftCM property

Расстояние от левого края клиентской области до левого края окна в сантиметрах.

```csharp
public double WindowLeftCM { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyWindowLeftCMDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Доступ к WorkbookSettings
            WorkbookSettings settings = workbook.Settings;

            // Установить свойство WindowLeftCM (расстояние от левого края экрана в сантиметрах)
            settings.WindowLeftCM = 2.54; // 1 inch = 2.54 cm

            // Проверьте настройку, распечатав её
            Console.WriteLine("WindowLeftCM: " + settings.WindowLeftCM);

            // Сохраните книгу
            workbook.Save("WindowLeftCMDemo.xlsx");
        }
    }
}
```

### См. также

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



---
title: "WorkbookSettings.WindowWidthCM"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство WorkbookSettings. Ширина окна в единицах сантиметров"
type: docs
url: /ru/net/aspose.cells/workbooksettings/windowwidthcm/
---
## WorkbookSettings.WindowWidthCM property

Ширина окна в сантиметрах.

```csharp
public double WindowWidthCM { get; set; }
```

### Примеры

```csharp
using System;
using System.Globalization;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyWindowWidthCMDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Доступ к WorkbookSettings
            WorkbookSettings settings = workbook.Settings;
            
            // Установить свойство WindowWidthCM (20,32 см = ~8 дюймов)
            settings.WindowWidthCM = 20.32;
            
            // Проверьте настройку, распечатав её
            Console.WriteLine("Window Width in Centimeters: " + settings.WindowWidthCM);
            
            // Сохраните книгу
            workbook.Save("WindowWidthCMDemo.xlsx");
        }
    }
}
```

### См. также

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



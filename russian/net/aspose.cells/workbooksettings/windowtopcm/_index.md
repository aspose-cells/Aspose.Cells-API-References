---
title: "WorkbookSettings.WindowTopCM"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство WorkbookSettings. Расстояние от верхнего края клиентской области до верхнего края окна в сантиметрах"
type: docs
url: /ru/net/aspose.cells/workbooksettings/windowtopcm/
---
## WorkbookSettings.WindowTopCM property

Расстояние от верхнего края клиентской области до верхнего края окна в сантиметрах.

```csharp
public double WindowTopCM { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyWindowTopCMDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Доступ к настройкам рабочей книги
            WorkbookSettings settings = workbook.Settings;

            // Установите свойство WindowTopCM (позиция от верхнего края в сантиметрах)
            settings.WindowTopCM = 2.5;

            // Отобразите текущее значение WindowTopCM
            Console.WriteLine("Window Top Position (cm): " + settings.WindowTopCM);

            // Сохраните книгу
            workbook.Save("WindowTopCMDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### См. также

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



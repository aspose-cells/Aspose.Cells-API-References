---
title: "WorkbookSettings.WindowLeftInch"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство WorkbookSettings. Расстояние от левого края клиентской области до левого края окна. В единицах дюйма"
type: docs
url: /ru/net/aspose.cells/workbooksettings/windowleftinch/
---
## WorkbookSettings.WindowLeftInch property

Расстояние от левого края клиентской области до левого края окна в дюймах.

```csharp
public double WindowLeftInch { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyWindowLeftInchDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Доступ к WorkbookSettings
            WorkbookSettings settings = workbook.Settings;

            // Установить свойство WindowLeftInch
            settings.WindowLeftInch = 1.5; // Position window 1.5 inches from left edge of screen

            // Добавьте некоторые примерные данные, чтобы продемонстрировать работоспособность книги
            Worksheet sheet = workbook.Worksheets[0];
            sheet.Cells["A1"].PutValue("Window Position Demo");
            sheet.Cells["A2"].PutValue($"Window left position: {settings.WindowLeftInch} inches");

            // Сохраните книгу
            workbook.Save("WindowLeftInchDemo.xlsx");

            Console.WriteLine("Workbook saved with WindowLeftInch = " + settings.WindowLeftInch);
        }
    }
}
```

### См. также

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



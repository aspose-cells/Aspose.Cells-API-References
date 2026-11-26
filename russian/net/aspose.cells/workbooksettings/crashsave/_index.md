---
title: "WorkbookSettings.CrashSave"
second_title: "Справочник API Aspose.Cells для .NET"
description: "WorkbookSettings property. указывает, сохраняло ли приложение файл рабочей книги после сбоя"
type: docs
url: /ru/net/aspose.cells/workbooksettings/crashsave/
---
## WorkbookSettings.CrashSave property

Указывает, сохранял ли приложение файл рабочей книги после сбоя.

```csharp
public bool CrashSave { get; set; }
```

### Примеры

```csharp
using System;
using System.Globalization;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyCrashSaveDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            sheet.Cells["A1"].PutValue("CrashSave Demo");
            sheet.Cells["A2"].PutValue(DateTime.Now);

            // Доступ к настройкам рабочей книги
            WorkbookSettings settings = workbook.Settings;

            // Продемонстрировать свойство CrashSave
            settings.CrashSave = true;
            Console.WriteLine($"CrashSave enabled: {settings.CrashSave}");

            // Сохранить с включённым сохранением после сбоя
            workbook.Save("CrashSaveEnabled.xlsx");

            // Отключить сохранение после сбоя
            settings.CrashSave = false;
            Console.WriteLine($"CrashSave enabled: {settings.CrashSave}");

            // Сохранить с отключённым сохранением после сбоя
            workbook.Save("CrashSaveDisabled.xlsx");
        }
    }
}
```

### См. также

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



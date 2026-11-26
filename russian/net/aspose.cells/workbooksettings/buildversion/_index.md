---
title: "WorkbookSettings.BuildVersion"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство WorkbookSettings. Указывает инкрементный публичный релиз приложения"
type: docs
url: /ru/net/aspose.cells/workbooksettings/buildversion/
---
## WorkbookSettings.BuildVersion property

Указывает инкрементальный публичный релиз приложения.

```csharp
public string BuildVersion { get; set; }
```

### Примеры

```csharp
using System;
using System.Globalization;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyBuildVersionDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Доступ к WorkbookSettings
            WorkbookSettings settings = workbook.Settings;
            
            // Установить базовые настройки
            settings.Author = "Sample Author";
            settings.CultureInfo = new CultureInfo("en-US");
            
            // Продемонстрировать свойство BuildVersion
            settings.BuildVersion = "2.5.0";
            Console.WriteLine($"Build Version set to: {settings.BuildVersion}");
            
            // Сохраните книгу
            workbook.Save("BuildVersionDemo.xlsx");
        }
    }
}
```

### См. также

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



---
title: "WorkbookSettings.EnableMacros"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство WorkbookSettings. Включить макросы"
type: docs
url: /ru/net/aspose.cells/workbooksettings/enablemacros/
---
## WorkbookSettings.EnableMacros property

Включить макросы;

```csharp
public bool EnableMacros { get; set; }
```

### Примечания

Теперь это работает только при копировании листа в другой лист в книге.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyEnableMacrosDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook wb = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet sheet = wb.Worksheets[0];
            
            // Добавьте примерные данные
            sheet.Cells["A1"].PutValue("Macro Test");
            
            // Продемонстрировать свойство EnableMacros
            Console.WriteLine("Initial EnableMacros value: " + wb.Settings.EnableMacros);
            
            // Отключить макросы
            wb.Settings.EnableMacros = false;
            Console.WriteLine("After disabling macros: " + wb.Settings.EnableMacros);
            
            // Включить макросы
            wb.Settings.EnableMacros = true;
            Console.WriteLine("After enabling macros: " + wb.Settings.EnableMacros);
            
            // Сохраните книгу
            wb.Save("EnableMacrosDemo.xlsx");
        }
    }
}
```

### См. также

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



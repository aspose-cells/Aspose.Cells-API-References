---
title: "WorkbookSettings.AutoRecover"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство WorkbookSettings. Указывает, помечен ли файл для автовосстановления"
type: docs
url: /ru/net/aspose.cells/workbooksettings/autorecover/
---
## WorkbookSettings.AutoRecover property

Указывает, помечен ли файл для автоматического восстановления.

```csharp
public bool AutoRecover { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyAutoRecoverDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Установите AutoRecover и другие параметры
            workbook.Settings.AutoRecover = false;
            workbook.Settings.DataExtractLoad = true;
            workbook.Settings.CrashSave = true;
            workbook.Settings.RepairLoad = true;

            // Сохраните книгу
            string outputPath = "WorkbookSettings_AutoRecoverDemo.xlsx";
            workbook.Save(outputPath);

            // Загрузить сохранённую книгу для проверки настроек
            Workbook loadedWorkbook = new Workbook(outputPath);
            
            // Выведите настройки в консоль
            Console.WriteLine("AutoRecover: " + loadedWorkbook.Settings.AutoRecover);
            Console.WriteLine("DataExtractLoad: " + loadedWorkbook.Settings.DataExtractLoad);
            Console.WriteLine("CrashSave: " + loadedWorkbook.Settings.CrashSave);
            Console.WriteLine("RepairLoad: " + loadedWorkbook.Settings.RepairLoad);
        }
    }
}
```

### См. также

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



---
title: "WorkbookSettings.RepairLoad"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство WorkbookSettings. Указывает, открыло ли приложение книгу в безопасном или режиме восстановления в последний раз"
type: docs
url: /ru/net/aspose.cells/workbooksettings/repairload/
---
## WorkbookSettings.RepairLoad property

Указывает, открыла ли приложение книгу в безопасном или режиме восстановления в последний раз.

```csharp
public bool RepairLoad { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyRepairLoadDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Настройте параметры книги
            workbook.Settings.AutoRecover = false;
            workbook.Settings.DataExtractLoad = true;
            workbook.Settings.CrashSave = true;
            workbook.Settings.RepairLoad = true;

            // Сохраните книгу
            string outputPath = "WorkbookSettings_RepairLoad_Example.xlsx";
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



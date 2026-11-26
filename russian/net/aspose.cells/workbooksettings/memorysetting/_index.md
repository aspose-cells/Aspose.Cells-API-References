---
title: "WorkbookSettings.MemorySetting"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство WorkbookSettings. Получает или задает параметры использования памяти. Новый параметр будет использоваться по умолчанию для только что созданных листов, но не будет применяться к существующим листам"
type: docs
url: /ru/net/aspose.cells/workbooksettings/memorysetting/
---
## WorkbookSettings.MemorySetting property

Получает или задает параметры использования памяти. Новый параметр будет использоваться как параметр по умолчанию для только что созданных листов, но не будет применяться к существующим листам.

```csharp
public MemorySetting MemorySetting { get; set; }
```

### Примечания

Для получения более подробной информации о режиме памяти, пожалуйста, смотрите [`MemorySetting`](../../cells/memorysetting/).

### Примеры

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyMemorySettingDemo
    {
        public static void Run()
        {
            // Создайте новую книгу с настройкой предпочтений памяти
            Workbook wb = new Workbook();
            wb.Settings.MemorySetting = MemorySetting.MemoryPreference;
            
            // Получить доступ к первому листу и добавить данные
            Worksheet sheet = wb.Worksheets[0];
            sheet.Cells["A1"].PutValue("Memory Setting Demo");
            sheet.Cells["A2"].PutValue(DateTime.Now.ToString());
            
            // Сохраните в поток памяти в формате PDF
            using (MemoryStream ms = new MemoryStream())
            {
                wb.Save(ms, SaveFormat.Pdf);
                Console.WriteLine("Workbook saved to PDF with MemoryPreference setting");
            }
        }
    }
}
```

### См. также

* enum [MemorySetting](../../memorysetting/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



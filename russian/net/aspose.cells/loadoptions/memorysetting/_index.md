---
title: "LoadOptions.MemorySetting"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство LoadOptions. Получает или задает режим памяти для загруженной книги"
type: docs
url: /ru/net/aspose.cells/loadoptions/memorysetting/
---
## LoadOptions.MemorySetting property

Получает или задает режим памяти для загруженной рабочей книги.

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
    public class LoadOptionsPropertyMemorySettingDemo
    {
        public static void Run()
        {
            // Создайте параметры загрузки с настройкой предпочтения памяти
            LoadOptions loadOptions = new LoadOptions(LoadFormat.Auto);
            loadOptions.MemorySetting = MemorySetting.MemoryPreference;

            // Загрузите книгу с оптимизированными настройками памяти
            Workbook workbook = new Workbook(new MemoryStream(), loadOptions);
            
            // Получить доступ к рабочему листу и добавить примерные данные
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Memory Setting Demo");
            worksheet.Cells["A2"].PutValue(DateTime.Now.ToString());
            
            // Сохраните книгу
            workbook.Save("MemorySettingDemo.xlsx", SaveFormat.Xlsx);
            
            Console.WriteLine("Workbook saved with MemoryPreference setting.");
        }
    }
}
```

### См. также

* enum [MemorySetting](../../memorysetting/)
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



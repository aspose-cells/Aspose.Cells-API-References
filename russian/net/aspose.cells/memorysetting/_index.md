---
title: "Перечисление MemorySetting"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.MemorySetting. Режимы использования памяти для модели данных ячеек"
type: docs
url: /ru/net/aspose.cells/memorysetting/
---
## MemorySetting enumeration

Режимы использования памяти для модели данных ячеек.

```csharp
public enum MemorySetting
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Normal | `0` | Режим по умолчанию для модели ячеек. |
| MemoryPreference | `1` | Предпочтительно производительность памяти. |
| FileCache | `2` | Предпочтительно производительность памяти и использование файла вместо памяти для хранения данных ячеек. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class MemorySettingDemo
    {
        public static void MemorySettingExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Получить доступ к настройкам книги
            WorkbookSettings settings = workbook.Settings;

            // Установите параметр использования памяти в MemoryPreference
            settings.MemorySetting = MemorySetting.MemoryPreference;

            // Создайте лист и добавьте некоторые данные
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["A2"].PutValue(123);

            // Сохраните книгу
            workbook.Save("MemorySettingExample.xlsx");

            Console.WriteLine("Workbook saved with MemorySetting.MemoryPreference.");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)



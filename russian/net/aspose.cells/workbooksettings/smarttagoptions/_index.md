---
title: "WorkbookSettings.SmartTagOptions"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство WorkbookSettings. Получает параметры смарт-тега"
type: docs
url: /ru/net/aspose.cells/workbooksettings/smarttagoptions/
---
## WorkbookSettings.SmartTagOptions property

Получает параметры смарт-тега.

```csharp
public SmartTagOptions SmartTagOptions { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertySmartTagOptionsDemo
    {
        public static void Run()
        {
            try
            {
                // Создать новую книгу
                Workbook workbook = new Workbook();

                // Получить доступ к настройкам книги
                WorkbookSettings settings = workbook.Settings;

                // Прочитайте свойство SmartTagOptions
                var smartTagOptions = settings.SmartTagOptions;

                // Отобразите информацию о экземпляре SmartTagOptions
                Console.WriteLine("SmartTagOptions instance type: " + smartTagOptions.GetType().FullName);

                // При желании вы можете просмотреть состояние по умолчанию с помощью ToString()
                Console.WriteLine("SmartTagOptions details: " + smartTagOptions.ToString());

                // Сохраните рабочую книгу (файл будет содержать настройки по умолчанию)
                workbook.Save("SmartTagOptionsDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [SmartTagOptions](../../../aspose.cells.markup/smarttagoptions/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



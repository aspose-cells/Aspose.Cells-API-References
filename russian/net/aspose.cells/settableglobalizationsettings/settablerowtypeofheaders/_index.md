---
title: "SettableGlobalizationSettings.SetTableRowTypeOfHeaders"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод SettableGlobalizationSettings. Устанавливает имя типа строк таблицы, которые представляют заголовок таблицы"
type: docs
url: /ru/net/aspose.cells/settableglobalizationsettings/settablerowtypeofheaders/
---
## SettableGlobalizationSettings.SetTableRowTypeOfHeaders method

Устанавливает имя типа строк таблицы, которые состоят из заголовка таблицы.

```csharp
public void SetTableRowTypeOfHeaders(string name)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| name | String | имя типа строк таблицы |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class SettableGlobalizationSettingsMethodSetTableRowTypeOfHeadersWithStringDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создать таблицу и добавить некоторые данные
            Cells cells = worksheet.Cells;
            cells["A1"].PutValue("Header1");
            cells["B1"].PutValue("Header2");
            cells["A2"].PutValue("Value1");
            cells["B2"].PutValue("Value2");
            
            // Создать объект ListObject (таблица)
            int index = worksheet.ListObjects.Add(0, 0, 1, 1, true);
            ListObject table = worksheet.ListObjects[index];
            table.ShowTotals = true;

            // Создать экземпляр SettableGlobalizationSettings
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();

            try
            {
                // Вызвать SetTableRowTypeOfHeaders с пользовательским именем типа заголовка
                settings.SetTableRowTypeOfHeaders("CustomHeaders");

                // Применить настройки к рабочей книге
                workbook.Settings.GlobalizationSettings = settings;

                Console.WriteLine("Table header type name set to: CustomHeaders");
                Console.WriteLine("In formulas, '#CustomHeaders' will now represent the table header");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetTableRowTypeOfHeaders method: {ex.Message}");
            }

            // Сохраните книгу
            workbook.Save("SetTableRowTypeOfHeadersDemo.xlsx");
        }
    }
}
```

### См. также

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



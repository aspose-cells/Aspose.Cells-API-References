---
title: "SettableGlobalizationSettings.SetTableRowTypeOfTotals"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод SettableGlobalizationSettings. Устанавливает имя типа строк таблицы, которые представляют итоговую строку ссылочной таблицы"
type: docs
url: /ru/net/aspose.cells/settableglobalizationsettings/settablerowtypeoftotals/
---
## SettableGlobalizationSettings.SetTableRowTypeOfTotals method

Устанавливает имя типа строк таблицы, которые состоят из итоговой строки ссылочной таблицы.

```csharp
public void SetTableRowTypeOfTotals(string name)
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

    public class SettableGlobalizationSettingsMethodSetTableRowTypeOfTotalsWithStringDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создать таблицу
            Cells cells = worksheet.Cells;
            cells["A1"].PutValue("Product");
            cells["B1"].PutValue("Price");
            cells["A2"].PutValue("Apple");
            cells["B2"].PutValue(10);
            cells["A3"].PutValue("Orange");
            cells["B3"].PutValue(15);
            cells["A4"].PutValue("Total");
            cells["B4"].PutValue("=SUM(B2:B3)");

            int tableIndex = worksheet.ListObjects.Add(0, 0, 3, 1, true);
            ListObject table = worksheet.ListObjects[tableIndex];
            table.ShowTotals = true;

            // Создать настройки глобализации
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();

            try
            {
                // Вызвать SetTableRowTypeOfTotals с пользовательским именем
                settings.SetTableRowTypeOfTotals("CustomTotals");

                // Применить настройки к рабочей книге
                workbook.Settings.GlobalizationSettings = settings;

                Console.WriteLine("SetTableRowTypeOfTotals executed successfully with parameter: CustomTotals");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetTableRowTypeOfTotals method: {ex.Message}");
            }

            // Сохраните книгу
            workbook.Save("SetTableRowTypeOfTotalsDemo.xlsx");
        }
    }
}
```

### См. также

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



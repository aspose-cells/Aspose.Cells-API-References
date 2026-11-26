---
title: "SettableGlobalizationSettings.SetTableRowTypeOfCurrent"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод SettableGlobalizationSettings. Устанавливает имя типа строк таблицы, которые состоят из текущей строки в ссылочной таблице"
type: docs
url: /ru/net/aspose.cells/settableglobalizationsettings/settablerowtypeofcurrent/
---
## SettableGlobalizationSettings.SetTableRowTypeOfCurrent method

Устанавливает имя типа строк таблицы, которые состоят из текущей строки в ссылочной таблице.

```csharp
public void SetTableRowTypeOfCurrent(string name)
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

    public class SettableGlobalizationSettingsMethodSetTableRowTypeOfCurrentWithStringDemo
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
            cells["B2"].PutValue("2.5");
            cells["A3"].PutValue("Banana");
            cells["B3"].PutValue("1.5");
            
            int tableIndex = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject table = worksheet.ListObjects[tableIndex];
            table.ShowTotals = true;
            table.ListColumns[1].TotalsCalculation = Aspose.Cells.Tables.TotalsCalculation.Sum;

            // Создать настройки глобализации
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
            
            try
            {
                // Установите пользовательское имя для типа текущей строки
                settings.SetTableRowTypeOfCurrent("CurrentItem");
                
                // Применить настройки к рабочей книге
                workbook.Settings.GlobalizationSettings = settings;

                // Проверьте настройку, получив значение обратно
                string currentRowType = settings.GetTableRowTypeOfCurrent();
                Console.WriteLine($"Current row type name set to: {currentRowType}");

                // Сохраните книгу
                workbook.Save("SetTableRowTypeOfCurrentDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetTableRowTypeOfCurrent method: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



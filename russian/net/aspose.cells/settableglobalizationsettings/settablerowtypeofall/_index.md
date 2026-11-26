---
title: "SettableGlobalizationSettings.SetTableRowTypeOfAll"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод SettableGlobalizationSettings. Устанавливает имя типа строк таблицы, которые состоят из всех строк в ссылочной таблице"
type: docs
url: /ru/net/aspose.cells/settableglobalizationsettings/settablerowtypeofall/
---
## SettableGlobalizationSettings.SetTableRowTypeOfAll method

Устанавливает имя типа строк таблицы, которые состоят из всех строк в ссылочной таблице.

```csharp
public void SetTableRowTypeOfAll(string name)
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

    public class SettableGlobalizationSettingsMethodSetTableRowTypeOfAllWithStringDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создайте примерные данные для таблицы
            Cells cells = worksheet.Cells;
            cells["A1"].PutValue("Product");
            cells["B1"].PutValue("Price");
            cells["A2"].PutValue("Apple");
            cells["B2"].PutValue(2.5);
            cells["A3"].PutValue("Orange");
            cells["B3"].PutValue(1.8);

            // Создать таблицу
            int tableIndex = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject table = worksheet.ListObjects[tableIndex];

            // Создайте пользовательские настройки глобализации
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();

            try
            {
                // Вызовите SetTableRowTypeOfAll с пользовательским именем
                settings.SetTableRowTypeOfAll("CompleteTable");

                // Применить настройки к рабочей книге
                workbook.Settings.GlobalizationSettings = settings;

                // Проверьте настройку, получив значение обратно
                string rowType = settings.GetTableRowTypeOfAll();
                Console.WriteLine($"Table row type for all rows set to: {rowType}");

                // Добавьте формулу, которая ссылается на все строки, используя пользовательское имя
                cells["C2"].Formula = "=SUM(#CompleteTable[Price])";
                Console.WriteLine($"Formula using custom row type: {cells["C2"].Formula}");

                // Вычислить формулы
                workbook.CalculateFormula();
                Console.WriteLine($"Calculation result: {cells["C2"].Value}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetTableRowTypeOfAll method: {ex.Message}");
            }

            // Сохраните книгу
            workbook.Save("MethodSetTableRowTypeOfAllWithStringDemo.xlsx");
        }
    }
}
```

### См. также

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



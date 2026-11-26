---
title: "SettableGlobalizationSettings.GetTableRowTypeOfCurrent"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод SettableGlobalizationSettings. Получает имя типа строк таблицы, которые состоят из текущей строки в ссылочной таблице"
type: docs
url: /ru/net/aspose.cells/settableglobalizationsettings/gettablerowtypeofcurrent/
---
## SettableGlobalizationSettings.GetTableRowTypeOfCurrent method

Получает название типа строк таблицы, состоящих из текущей строки в ссылочной таблице.

```csharp
public override string GetTableRowTypeOfCurrent()
```

### Возвращаемое значение

имя типа строк таблицы

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class SettableGlobalizationSettingsMethodGetTableRowTypeOfCurrentDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создать таблицу
            Cells cells = worksheet.Cells;
            cells["A1"].PutValue("Name");
            cells["B1"].PutValue("Age");
            cells["A2"].PutValue("John");
            cells["B2"].PutValue(30);
            cells["A3"].PutValue("Alice");
            cells["B3"].PutValue(25);

            int tableIndex = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject table = worksheet.ListObjects[tableIndex];
            table.ShowTotals = true;
            table.ListColumns[1].TotalsCalculation = Aspose.Cells.Tables.TotalsCalculation.Sum;

            // Создайте пользовательские настройки глобализации
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
            settings.SetTableRowTypeOfCurrent("CurrentRow");

            // Применить настройки к рабочей книге
            workbook.Settings.GlobalizationSettings = settings;

            try
            {
                // Получить имя типа текущей строки
                string currentRowType = settings.GetTableRowTypeOfCurrent();
                Console.WriteLine("Current row type name: " + currentRowType);

                // Добавить формулу, ссылающуюся на текущую строку
                cells["C2"].Formula = "=SUM(#CurrentRow)";
                Console.WriteLine("Formula set to: " + cells["C2"].Formula);

                // Вычислить формулы
                workbook.CalculateFormula();
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetTableRowTypeOfCurrent method: {ex.Message}");
            }

            // Сохранить результат
            workbook.Save("MethodGetTableRowTypeOfCurrentDemo.xlsx");
        }
    }
}
```

### См. также

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



---
title: "SettableGlobalizationSettings.GetTableRowTypeOfTotals"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод SettableGlobalizationSettings. Получает имя типа строк таблицы, которые состоят из итоговой строки указанной таблицы"
type: docs
url: /ru/net/aspose.cells/settableglobalizationsettings/gettablerowtypeoftotals/
---
## SettableGlobalizationSettings.GetTableRowTypeOfTotals method

Получает имя типа строк таблицы, которые состоят из итоговой строки ссылочной таблицы.

```csharp
public override string GetTableRowTypeOfTotals()
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

    public class SettableGlobalizationSettingsMethodGetTableRowTypeOfTotalsDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создать примерные данные таблицы
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B3"].PutValue(15);
            worksheet.Cells["A4"].PutValue("Total");
            worksheet.Cells["B4"].PutValue("=SUM(B2:B3)");

            // Создать объект ListObject (таблица)
            int index = worksheet.ListObjects.Add(0, 0, 3, 1, true);
            ListObject table = worksheet.ListObjects[index];
            table.ShowTotals = true;

            // Создайте пользовательские настройки глобализации
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
            settings.SetTableRowTypeOfTotals("CustomTotals");

            try
            {
                // Получить тип строки таблицы для итогов
                string rowType = settings.GetTableRowTypeOfTotals();
                Console.WriteLine($"Table row type for totals: {rowType}");

                // Применить настройки к рабочей книге
                workbook.Settings.GlobalizationSettings = settings;

                // Проверить эффект в формуле
                worksheet.Cells["C2"].Formula = "=SUM(#CustomTotals[B])";
                Console.WriteLine("Formula using custom totals reference: " + worksheet.Cells["C2"].Formula);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetTableRowTypeOfTotals method: {ex.Message}");
            }

            // Сохранить результат
            workbook.Save("MethodGetTableRowTypeOfTotalsDemo.xlsx");
        }
    }
}
```

### См. также

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



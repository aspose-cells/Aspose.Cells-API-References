---
title: "GlobalizationSettings.GetTableRowTypeOfCurrent"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод GlobalizationSettings. Получает имя типа строк таблицы, которые состоят из текущей строки в ссылочной таблице. По умолчанию это This Row, поэтому в формуле This Row представляет текущую строку в ссылочной таблице."
type: docs
url: /ru/net/aspose.cells/globalizationsettings/gettablerowtypeofcurrent/
---
## GlobalizationSettings.GetTableRowTypeOfCurrent method

Получает название типа строк таблицы, которые состоят из текущей строки в ссылочной таблице. По умолчанию "This Row", поэтому в формуле "#This Row" представляет текущую строку в ссылочной таблице.

```csharp
public virtual string GetTableRowTypeOfCurrent()
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

    public class GlobalizationSettingsMethodGetTableRowTypeOfCurrentDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Установить пользовательские настройки глобализации
            workbook.Settings.GlobalizationSettings = new CustomGlobalizationSettings();

            try
            {
                // Создайте примерные данные и таблицу
                worksheet.Cells["A1"].PutValue("Product");
                worksheet.Cells["B1"].PutValue("Price");
                worksheet.Cells["A2"].PutValue("Apple");
                worksheet.Cells["B2"].PutValue(2.5);
                worksheet.Cells["A3"].PutValue("Orange");
                worksheet.Cells["B3"].PutValue(1.8);

                // Создайте таблицу
                int tableIndex = worksheet.ListObjects.Add(0, 0, 2, 1, true);
                ListObject table = worksheet.ListObjects[tableIndex];
                table.DisplayName = "PriceTable"; // Fixed property name

                // Добавьте формулу, используя ссылку на текущую строку
                Cell formulaCell = worksheet.Cells["C2"];
                formulaCell.Formula = "=PriceTable[@Price] * 1.2";

                // Продемонстрируйте эффект GetTableRowTypeOfCurrent
                Console.WriteLine("Generated formula: " + formulaCell.Formula);
                Console.WriteLine("Method executed successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetTableRowTypeOfCurrent method: {ex.Message}");
            }

            // Сохраните книгу
            workbook.Save("MethodGetTableRowTypeOfCurrentDemo.xlsx");
        }
    }

    public class CustomGlobalizationSettings : GlobalizationSettings
    {
        public override string GetTableRowTypeOfCurrent()
        {
            return "CurrentItem"; // Custom current row identifier
        }
    }
}
```

### См. также

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



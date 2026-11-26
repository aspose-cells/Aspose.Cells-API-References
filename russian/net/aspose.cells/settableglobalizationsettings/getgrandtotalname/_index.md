---
title: "SettableGlobalizationSettings.GetGrandTotalName"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод SettableGlobalizationSettings. Получает название общего итога функции"
type: docs
url: /ru/net/aspose.cells/settableglobalizationsettings/getgrandtotalname/
---
## SettableGlobalizationSettings.GetGrandTotalName method

Получает название общего итога функции.

```csharp
public override string GetGrandTotalName(ConsolidationFunction functionType)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| functionType | ConsolidationFunction | Тип функции. |

### Возвращаемое значение

Имя общего итога функции.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot; // Added this using directive
    using System;

    public class SettableGlobalizationSettingsMethodGetGrandTotalNameWithConsolidationFunctionDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создайте пользовательские настройки глобализации
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
            
            // Установите пользовательские названия общего итога для разных функций консолидации
            settings.SetGrandTotalName(ConsolidationFunction.Sum, "Custom Sum Grand Total");
            settings.SetGrandTotalName(ConsolidationFunction.Average, "Custom Average Grand Total");
            
            // Применить настройки к рабочей книге
            workbook.Settings.GlobalizationSettings = settings;

            try
            {
                // Вызовите GetGrandTotalName с разными функциями консолидации
                string sumGrandTotalName = settings.GetGrandTotalName(ConsolidationFunction.Sum);
                string avgGrandTotalName = settings.GetGrandTotalName(ConsolidationFunction.Average);
                
                // Выведите результаты
                Console.WriteLine("Sum Grand Total Name: " + sumGrandTotalName);
                Console.WriteLine("Average Grand Total Name: " + avgGrandTotalName);

                // Создайте сводную таблицу, чтобы продемонстрировать эффект
                Cells cells = worksheet.Cells;
                cells["A1"].PutValue("Product");
                cells["B1"].PutValue("Sales");
                cells["A2"].PutValue("Apple");
                cells["B2"].PutValue(1000);
                cells["A3"].PutValue("Orange");
                cells["B3"].PutValue(2000);
                cells["A4"].PutValue("Banana");
                cells["B4"].PutValue(3000);

                PivotTableCollection pivotTables = worksheet.PivotTables;
                int index = pivotTables.Add("A1:B4", "E3", "PivotTable1");
                PivotTable pivotTable = pivotTables[index];
                pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
                pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
                pivotTable.DataFields[0].Function = ConsolidationFunction.Sum;
                
                // Правильный способ добавить еще одно поле данных с функцией Average
                pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
                pivotTable.DataFields[1].Function = ConsolidationFunction.Average;
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetGrandTotalName method: {ex.Message}");
            }
            
            // Сохраните книгу
            workbook.Save("SettableGlobalizationSettingsMethodGetGrandTotalNameDemo.xlsx");
        }
    }
}
```

### См. также

* enum [ConsolidationFunction](../../consolidationfunction/)
* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



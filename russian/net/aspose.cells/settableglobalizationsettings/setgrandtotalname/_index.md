---
title: "SettableGlobalizationSettings.SetGrandTotalName"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод SettableGlobalizationSettings. Устанавливает имя общего итога для конкретной функции"
type: docs
url: /ru/net/aspose.cells/settableglobalizationsettings/setgrandtotalname/
---
## SettableGlobalizationSettings.SetGrandTotalName method

Устанавливает имя общего итога конкретной функции.

```csharp
public void SetGrandTotalName(ConsolidationFunction functionType, string name)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| functionType | ConsolidationFunction | Тип функции. |
| name | String | Имя общего итога функции. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class SettableGlobalizationSettingsMethodSetGrandTotalNameWithConsolidationFunctionStringDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создать примерные данные для сводной таблицы
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Fruit");
            worksheet.Cells["A3"].PutValue("Fruit");
            worksheet.Cells["A4"].PutValue("Vegetable");
            worksheet.Cells["B1"].PutValue("Amount");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(50);
            worksheet.Cells["B4"].PutValue(75);

            // Создать сводную таблицу
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            pivotTable.DataFields[0].Function = ConsolidationFunction.Sum;

            // Создайте пользовательские настройки глобализации
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
            workbook.Settings.GlobalizationSettings = settings;

            try
            {
                // Вызовите SetGrandTotalName с ConsolidationFunction.Sum и пользовательским именем
                settings.SetGrandTotalName(ConsolidationFunction.Sum, "Custom Grand Total");

                // Обновить сводную таблицу, чтобы применить изменения
                pivotTable.RefreshData();
                pivotTable.CalculateData();

                Console.WriteLine("Grand total name set to 'Custom Grand Total' for Sum function");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetGrandTotalName method: {ex.Message}");
            }

            // Сохраните книгу
            workbook.Save("MethodSetGrandTotalNameDemo.xlsx");
        }
    }
}
```

### См. также

* enum [ConsolidationFunction](../../consolidationfunction/)
* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



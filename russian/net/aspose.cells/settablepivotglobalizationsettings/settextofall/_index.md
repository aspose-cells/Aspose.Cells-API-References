---
title: "SettablePivotGlobalizationSettings.SetTextOfAll"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод SettablePivotGlobalizationSettings. Устанавливает текст метки All в сводной таблице"
type: docs
url: /ru/net/aspose.cells/settablepivotglobalizationsettings/settextofall/
---
## SettablePivotGlobalizationSettings.SetTextOfAll method

Устанавливает текст метки "(All)" в сводной таблице.

```csharp
public void SetTextOfAll(string text)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| текст | String | пользовательский текст |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class SettablePivotGlobalizationSettingsMethodSetTextOfAllWithStringDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные для сводной таблицы
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["B4"].PutValue(3000);

            // Создать сводную таблицу
            var pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            var pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Создать настройки глобализации
            var settings = new SettableGlobalizationSettings();
            settings.PivotSettings = new SettablePivotGlobalizationSettings();

            try
            {
                // Вызовите метод SetTextOfAll, чтобы изменить текст "(All)"
                ((SettablePivotGlobalizationSettings)settings.PivotSettings).SetTextOfAll("All Products");

                // Применить настройки к рабочей книге
                workbook.Settings.GlobalizationSettings = settings;
                pivotTable.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium2;

                Console.WriteLine("SetTextOfAll method executed successfully. Changed '(All)' to 'All Products'");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetTextOfAll method: {ex.Message}");
            }

            // Сохранить результат
            workbook.Save("SettablePivotGlobalizationSettingsMethodSetTextOfAllDemo.xlsx");
        }
    }
}
```

### См. также

* class [SettablePivotGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



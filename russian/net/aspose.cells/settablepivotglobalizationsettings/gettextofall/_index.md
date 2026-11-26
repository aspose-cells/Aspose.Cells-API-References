---
title: "SettablePivotGlobalizationSettings.GetTextOfAll"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод SettablePivotGlobalizationSettings. Получает текст метки All в сводной таблице"
type: docs
url: /ru/net/aspose.cells/settablepivotglobalizationsettings/gettextofall/
---
## SettablePivotGlobalizationSettings.GetTextOfAll method

Получает текст метки "(All)" в сводной таблице.

```csharp
public override string GetTextOfAll()
```

### Возвращаемое значение

Текст метки "(All)"

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class SettablePivotGlobalizationSettingsMethodGetTextOfAllDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создать примерные данные для сводной таблицы
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("A");
            worksheet.Cells["B4"].PutValue(15);

            // Создать сводную таблицу
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Создать настройки глобализации
            SettablePivotGlobalizationSettings settings = new SettablePivotGlobalizationSettings();
            settings.SetTextOfAll("(All Items)");

            try
            {
                // Получить текущий текст метки "(All)"
                string currentText = settings.GetTextOfAll();
                Console.WriteLine($"Current text of '(All)' label: {currentText}");

                // Обновить сводную таблицу с новыми настройками
                pivotTable.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium2;
                pivotTable.RefreshData();
                pivotTable.CalculateData();

                Console.WriteLine("Method executed successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetTextOfAll method: {ex.Message}");
            }

            // Сохранить результат
            workbook.Save("MethodGetTextOfAllDemo.xlsx");
        }
    }
}
```

### См. также

* class [SettablePivotGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



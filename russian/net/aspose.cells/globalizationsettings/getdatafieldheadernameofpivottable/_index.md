---
title: "GlobalizationSettings.GetDataFieldHeaderNameOfPivotTable"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод GlobalizationSettings. Получает название заголовка поля области значений в сводной таблице"
type: docs
url: /ru/net/aspose.cells/globalizationsettings/getdatafieldheadernameofpivottable/
---
## GlobalizationSettings.GetDataFieldHeaderNameOfPivotTable method

Получает название заголовка поля области значений в сводной таблице.

```csharp
[Obsolete("Use PivotGlobalizationSettings.GetTextOfDataFieldHeader() method instead.")]
public virtual string GetDataFieldHeaderNameOfPivotTable()
```

### Возвращаемое значение

Название заголовка поля данных

### Примечания

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него, пожалуйста, используйте метод PivotGlobalizationSettings.GetColumnLabelsOfPivotTable(). Это свойство будет удалено через 12 месяцев, начиная с декабря 2022 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class GlobalizationSettingsMethodGetDataFieldHeaderNameOfPivotTableDemo
    {
        public static void Run()
        {
            // Создайте новую книгу и получите доступ к первому листу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные для сводной таблицы
            worksheet.Cells["A1"].Value = "Category";
            worksheet.Cells["B1"].Value = "Value";
            worksheet.Cells["A2"].Value = "A";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["A3"].Value = "B";
            worksheet.Cells["B3"].Value = 200;

            // Установить пользовательские настройки глобализации
            workbook.Settings.GlobalizationSettings = new CustomGlobalizationSettings();

            try
            {
                // Создать сводную таблицу и настроить поля
                int pivotIndex = worksheet.PivotTables.Add("PivotTable", "A1:B3", "D1");
                PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
                pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Category as row
                pivotTable.AddFieldToArea(PivotFieldType.Data, 1);  // Value as data

                // Обновить сводную таблицу, чтобы применить изменения локализации
                pivotTable.RefreshData();
                pivotTable.CalculateData();

                Console.WriteLine("PivotTable created with custom data field header name.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }

            // Сохранить изменённую книгу
            workbook.Save("GlobalizationSettingsMethodDemo.xlsx");
        }
    }

    // Пользовательская реализация GlobalizationSettings
    public class CustomGlobalizationSettings : GlobalizationSettings
    {
        public override string GetDataFieldHeaderNameOfPivotTable()
        {
            return "Custom Values";
        }
    }
}
```

### См. также

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



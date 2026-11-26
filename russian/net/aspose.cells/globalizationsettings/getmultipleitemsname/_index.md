---
title: "GlobalizationSettings.GetMultipleItemsName"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод GlobalizationSettings. Получает название метки Multiple Items в сводной таблице"
type: docs
url: /ru/net/aspose.cells/globalizationsettings/getmultipleitemsname/
---
## GlobalizationSettings.GetMultipleItemsName method

Получает название метки "(Multiple Items)" в сводной таблице.

```csharp
[Obsolete("Use PivotGlobalizationSettings.GetTextOfMultipleItems() method instead.")]
public virtual string GetMultipleItemsName()
```

### Возвращаемое значение

Название метки "(Multiple Items)"

### Примечания

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него, пожалуйста, используйте метод PivotGlobalizationSettings.GetColumnLabelsOfPivotTable(). Это свойство будет удалено через 12 месяцев, начиная с декабря 2022 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class GlobalizationSettingsMethodGetMultipleItemsNameDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Подготовить примерные данные для сводной таблицы
            worksheet.Cells["A1"].Value = "Category";
            worksheet.Cells["A2"].Value = "A";
            worksheet.Cells["A3"].Value = "B";
            worksheet.Cells["A4"].Value = "C";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["B3"].Value = 200;
            worksheet.Cells["B4"].Value = 300;

            // Создать сводную таблицу
            int pivotIndex = worksheet.PivotTables.Add("D1", "A1:B4", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);

            // Настроить PivotField для отображения нескольких элементов
            PivotField rowField = pivotTable.RowFields[0];
            rowField.IsMultipleItemSelectionAllowed = true;
            rowField.HideItem(0, false); // Select "A"
            rowField.HideItem(1, false); // Select "B"

            // Инициализировать настройки глобализации
            GlobalizationSettings gSettings = workbook.Settings.GlobalizationSettings ?? new GlobalizationSettings();
            workbook.Settings.GlobalizationSettings = gSettings;

            try
            {
                // Вызвать GetMultipleItemsName и отобразить результат
                string multipleItemsName = gSettings.GetMultipleItemsName();
                Console.WriteLine($"Multiple Items Name: {multipleItemsName}");

                // Обновить сводную таблицу, чтобы применить настройки
                pivotTable.RefreshData();
                pivotTable.CalculateData();
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetMultipleItemsName: {ex.Message}");
            }

            // Сохранить книгу, чтобы показать сводную таблицу с меткой нескольких элементов
            workbook.Save("GlobalizationSettingsMethodGetMultipleItemsNameDemo.xlsx");
        }
    }
}
```

### См. также

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



---
title: "GlobalizationSettings.GetColumnLabelsOfPivotTable"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод GlobalizationSettings. Получает название метки Column Labels в сводной таблице."
type: docs
url: /ru/net/aspose.cells/globalizationsettings/getcolumnlabelsofpivottable/
---
## GlobalizationSettings.GetColumnLabelsOfPivotTable method

Получает имя метки "Column Labels" в сводной таблице.

```csharp
[Obsolete("Use PivotGlobalizationSettings.GetTextOfColumnLabels() method instead.")]
public virtual string GetColumnLabelsOfPivotTable()
```

### Возвращаемое значение

Имя меток столбцов

### Примечания

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него, пожалуйста, используйте метод PivotGlobalizationSettings.GetColumnLabelsOfPivotTable(). Это свойство будет удалено через 12 месяцев, начиная с декабря 2022 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class GlobalizationSettingsMethodGetColumnLabelsOfPivotTableDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Заполнить примерными данными сводную таблицу
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["B1"].Value = "Region";
            worksheet.Cells["C1"].Value = "Sales";
            worksheet.Cells["A2"].Value = "Bike";
            worksheet.Cells["B2"].Value = "North";
            worksheet.Cells["C2"].Value = 10000;
            worksheet.Cells["A3"].Value = "Bike";
            worksheet.Cells["B3"].Value = "South";
            worksheet.Cells["C3"].Value = 8000;
            worksheet.Cells["A4"].Value = "Car";
            worksheet.Cells["B4"].Value = "North";
            worksheet.Cells["C4"].Value = 25000;

            // Создать сводную таблицу и получить ссылку
            int pivotTableIndex = worksheet.PivotTables.Add("PivotTable", "A1:C4", "E5");
            PivotTable pivotTable = worksheet.PivotTables[pivotTableIndex];
            
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Product
            pivotTable.AddFieldToArea(PivotFieldType.Column, 1); // Region
            pivotTable.AddFieldToArea(PivotFieldType.Data, 2); // Sales

            // Применить пользовательские настройки глобализации для переопределения меток столбцов
            workbook.Settings.GlobalizationSettings = new CustomGlobalizationSettings();

            try
            {
                // Обновить и вычислить сводную таблицу для применения настроек
                pivotTable.RefreshData();
                pivotTable.CalculateData();

                Console.WriteLine("GetColumnLabelsOfPivotTable method executed successfully. Check 'output.xlsx'.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }

            // Сохраните книгу
            workbook.Save("output.xlsx");
        }
    }

    // Пользовательская реализация GlobalizationSettings для переопределения меток столбцов
    public class CustomGlobalizationSettings : GlobalizationSettings
    {
        public override string GetColumnLabelsOfPivotTable()
        {
            // Вернуть пользовательскую метку для заголовков столбцов сводной таблицы
            return "Sales Regions";
        }
    }
}
```

### См. также

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



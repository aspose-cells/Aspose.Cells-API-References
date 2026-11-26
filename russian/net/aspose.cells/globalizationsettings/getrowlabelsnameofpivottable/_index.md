---
title: "GlobalizationSettings.GetRowLabelsNameOfPivotTable"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод GlobalizationSettings. Получает имя метки Row Labels в PivotTable"
type: docs
url: /ru/net/aspose.cells/globalizationsettings/getrowlabelsnameofpivottable/
---
## GlobalizationSettings.GetRowLabelsNameOfPivotTable method

Получает имя метки "Row Labels" в PivotTable.

```csharp
[Obsolete("Use PivotGlobalizationSettings.GetTextOfRowLabels() method instead.")]
public virtual string GetRowLabelsNameOfPivotTable()
```

### Возвращаемое значение

Имя меток строк

### Примечания

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него, пожалуйста, используйте метод PivotGlobalizationSettings.GetColumnLabelsOfPivotTable(). Это свойство будет удалено через 12 месяцев, начиная с декабря 2022 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class CustomGlobalizationSettings : GlobalizationSettings
    {
        public override string GetRowLabelsNameOfPivotTable()
        {
            return "Custom Row Labels";
        }
    }

    public class GlobalizationSettingsMethodGetRowLabelsNameOfPivotTableDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создать примерные данные для сводной таблицы
            Cells cells = worksheet.Cells;
            cells["A1"].PutValue("Product");
            cells["A2"].PutValue("Bikes");
            cells["A3"].PutValue("Cars");
            cells["B1"].PutValue("Sales");
            cells["B2"].PutValue(1000);
            cells["B3"].PutValue(2500);

            // Создать сводную таблицу
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int pivotIndex = pivotTables.Add("A1:B3", "E3", "SalesPivot");
            PivotTable pivotTable = pivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Product as row field

            // Применить пользовательские параметры глобализации
            workbook.Settings.GlobalizationSettings = new CustomGlobalizationSettings();

            try
            {
                pivotTable.RefreshData();
                pivotTable.CalculateData();
                Console.WriteLine("Pivot table created with custom row labels name.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetRowLabelsNameOfPivotTable: {ex.Message}");
            }

            workbook.Save("GlobalizationSettingsMethodGetRowLabelsNameOfPivotTableDemo.xlsx");
        }
    }
}
```

### См. также

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



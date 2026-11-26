---
title: "GlobalizationSettings.GetPivotTotalName"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод GlobalizationSettings. Получает имя метки \"Total\" в сводной таблице. Вам необходимо переопределить этот метод, когда в области данных сводной таблицы содержится два или более полей PivotFields."
type: docs
url: /ru/net/aspose.cells/globalizationsettings/getpivottotalname/
---
## GlobalizationSettings.GetPivotTotalName method

Получает имя метки "Total" в сводной таблице. Вам необходимо переопределить этот метод, когда в области данных сводной таблицы содержится два или более полей PivotFields.

```csharp
[Obsolete("Use PivotGlobalizationSettings.GetTextOfTotal() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public virtual string GetPivotTotalName()
```

### Возвращаемое значение

Имя метки "Total"

### Примечания

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него, пожалуйста, используйте метод PivotGlobalizationSettings.GetColumnLabelsOfPivotTable(). Это свойство будет удалено через 12 месяцев, начиная с декабря 2022 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class GlobalizationSettingsMethodGetPivotTotalNameDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Заполнить примерными данными
            worksheet.Cells["A1"].Value = "Region";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["C1"].Value = "Quantity";
            worksheet.Cells["A2"].Value = "North"; worksheet.Cells["B2"].Value = 1000; worksheet.Cells["C2"].Value = 50;
            worksheet.Cells["A3"].Value = "South"; worksheet.Cells["B3"].Value = 2000; worksheet.Cells["C3"].Value = 70;
            worksheet.Cells["A4"].Value = "West"; worksheet.Cells["B4"].Value = 3000; worksheet.Cells["C4"].Value = 110;

            // Создать сводную таблицу
            int pivotIndex = worksheet.PivotTables.Add("A1:C4", "E5", "SalesPivot");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Region
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Sales
            pivotTable.AddFieldToArea(PivotFieldType.Data, 2); // Quantity

            // Создать и настроить параметры глобализации
            var customSettings = new CustomGlobalizationSettings();
            workbook.Settings.GlobalizationSettings = customSettings;

            try
            {
                // Демонстрировать прямой вызов метода
                Console.WriteLine("Custom Total Name: " + customSettings.GetPivotTotalName());

                // Обработать сводную таблицу
                pivotTable.RefreshData();
                pivotTable.CalculateData();

                Console.WriteLine("Pivot table created with custom total name.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }

            workbook.Save("MethodGetPivotTotalNameDemo.xlsx");
        }
    }

    public class CustomGlobalizationSettings : GlobalizationSettings
    {
        public override string GetPivotTotalName()
        {
            return "Custom Total";
        }
    }
}
```

### См. также

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



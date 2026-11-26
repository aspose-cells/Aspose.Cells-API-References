---
title: "GlobalizationSettings.GetPivotGrandTotalName"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод GlobalizationSettings. Получает имя метки Grand Total в сводной таблице"
type: docs
url: /ru/net/aspose.cells/globalizationsettings/getpivotgrandtotalname/
---
## GlobalizationSettings.GetPivotGrandTotalName method

Получает имя метки "Grand Total" в сводной таблице.

```csharp
[Obsolete("Use PivotGlobalizationSettings.GetTextOfGrandTotal() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public virtual string GetPivotGrandTotalName()
```

### Возвращаемое значение

Имя метки "Grand Total"

### Примечания

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него, пожалуйста, используйте метод PivotGlobalizationSettings.GetColumnLabelsOfPivotTable(). Это свойство будет удалено через 12 месяцев, начиная с декабря 2022 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class GlobalizationSettingsMethodGetPivotGrandTotalNameDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Установить пользовательские настройки глобализации
            var settings = new CustomGlobalizationSettings();
            workbook.Settings.GlobalizationSettings = settings;

            // Заполните сводную таблицу примерными данными
            var cells = worksheet.Cells;
            cells["A1"].Value = "Category";
            cells["B1"].Value = "Q1";
            cells["C1"].Value = "Q2";
            cells["A2"].Value = "Electronics";
            cells["B2"].Value = 1500;
            cells["C2"].Value = 2200;
            cells["A3"].Value = "Clothing";
            cells["B3"].Value = 900;
            cells["C3"].Value = 1300;

            // Создайте сводную таблицу с несколькими полями данных
            int pivotTableIndex = worksheet.PivotTables.Add("PivotTable", "A1:C3", "E4");
            PivotTable pivotTable = worksheet.PivotTables[pivotTableIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Category
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Q1
            pivotTable.AddFieldToArea(PivotFieldType.Data, 2); // Q2

            // Обновить и вычислить сводную таблицу
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            try
            {
                // Продемонстрировать вызов GetPivotGrandTotalName
                string grandTotalName = settings.GetPivotGrandTotalName();
                Console.WriteLine($"Custom Grand Total Name: {grandTotalName}");

                // Сохранить изменённую книгу
                workbook.Save("GlobalizationSettingsMethodGetPivotGrandTotalNameDemo.xlsx");
                Console.WriteLine("Spreadsheet saved. Check output file.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing demo: {ex.Message}");
            }
        }

        private class CustomGlobalizationSettings : GlobalizationSettings
        {
            public override string GetPivotGrandTotalName()
            {
                return "[Custom Grand Total]";
            }
        }
    }
}
```

### См. также

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



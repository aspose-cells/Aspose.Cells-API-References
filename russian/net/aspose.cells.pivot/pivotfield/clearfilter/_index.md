---
title: "PivotField.ClearFilter"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод PivotField. Очищает настройку фильтра для этого поля сводки"
type: docs
url: /ru/net/aspose.cells.pivot/pivotfield/clearfilter/
---
## PivotField.ClearFilter method

Очищает настройки фильтра для этого сводного поля.

```csharp
public void ClearFilter()
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldMethodClearFilterDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные для сводной таблицы
            worksheet.Cells["A1"].Value = "Category";
            worksheet.Cells["A2"].Value = "Fruit";
            worksheet.Cells["A3"].Value = "Vegetable";
            worksheet.Cells["A4"].Value = "Fruit";
            worksheet.Cells["A5"].Value = "Vegetable";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["B3"].Value = 200;
            worksheet.Cells["B4"].Value = 150;
            worksheet.Cells["B5"].Value = 300;

            // Создать сводную таблицу
            int pivotIndex = worksheet.PivotTables.Add("A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Добавить поле строки
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            
            // Добавить поле данных
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Получить поле сводной таблицы
            PivotField pivotField = pivotTable.RowFields[0];

            try
            {
                // Сначала примените фильтр, чтобы продемонстрировать его очистку
                pivotField.FilterByLabel(PivotFilterType.CaptionEqual, "Fruit", null);

                // Вызовите метод ClearFilter
                pivotField.ClearFilter();

                Console.WriteLine("ClearFilter method executed successfully");
                Console.WriteLine("All filters have been removed from the pivot field");

                // Обновите сводную таблицу, чтобы отобразить изменения
                pivotTable.RefreshData();
                pivotTable.CalculateData();
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ClearFilter method: {ex.Message}");
            }

            // Сохранить результат
            workbook.Save("PivotFieldMethodClearFilterDemo.xlsx");
        }
    }
}
```

### См. также

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)



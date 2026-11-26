---
title: "PivotTable.ChangeDataSource"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод PivotTable. Изменить источник данных сводной таблицы"
type: docs
url: /ru/net/aspose.cells.pivot/pivottable/changedatasource/
---
## PivotTable.ChangeDataSource method

Изменить источник данных сводной таблицы.

```csharp
public void ChangeDataSource(string[] source)
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot; // Added this using directive
    using System;

    public class PivotTableMethodChangeDataSourceWithStringDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте образцовые данные для сводной таблицы
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["A4"].PutValue("Orange");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["B4"].PutValue(3000);

            // Создайте сводную таблицу
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];

            // Добавьте поля в сводную таблицу
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Подготовить новый источник данных
            string[] newDataSource = new string[] { "C1:D4", "Sheet1" };

            try
            {
                // Изменить источник данных сводной таблицы
                pivotTable.ChangeDataSource(newDataSource);

                // Обновить сводную таблицу, чтобы применить изменения
                pivotTable.RefreshData();
                pivotTable.CalculateData();

                Console.WriteLine("PivotTable data source changed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error changing pivot table data source: {ex.Message}");
            }

            // Сохраните книгу
            workbook.Save("PivotTableChangeDataSourceDemo.xlsx");
        }
    }
}
```

### См. также

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)



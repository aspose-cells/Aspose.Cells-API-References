---
title: "PivotField.InitPivotItems"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод PivotField. Инициализирует элементы сводки поля"
type: docs
url: /ru/net/aspose.cells.pivot/pivotfield/initpivotitems/
---
## PivotField.InitPivotItems method

Инициализировать элементы сводки поля

```csharp
[Obsolete("Please simply remove calling this method.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void InitPivotItems()
```

### Примечания

ПРИМЕЧАНИЕ: Этот метод теперь устарел. Пожалуйста, просто перестаньте вызывать этот метод. Этот метод будет удалён через 6 месяцев, начиная с октября 2026 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldMethodInitPivotItemsDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте образцовые данные для сводной таблицы
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("Bike");
            worksheet.Cells["A3"].PutValue("Car");
            worksheet.Cells["A4"].PutValue("Bike");
            worksheet.Cells["A5"].PutValue("Car");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["B4"].PutValue(1500);
            worksheet.Cells["B5"].PutValue(2500);

            // Создайте сводную таблицу
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int index = pivotTables.Add("A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];

            // Добавить поле строки
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");

            // Получить поле сводной таблицы
            PivotField pivotField = pivotTable.RowFields[0];

            try
            {
                // Инициализировать элементы сводки
                pivotField.InitPivotItems();

                // Отобразить элементы сводки
                Console.WriteLine("Pivot Items after initialization:");
                foreach (PivotItem item in pivotField.PivotItems)
                {
                    Console.WriteLine(item.Name);
                }

                // Сохраните книгу
                workbook.Save("PivotFieldInitPivotItemsDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing InitPivotItems method: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)



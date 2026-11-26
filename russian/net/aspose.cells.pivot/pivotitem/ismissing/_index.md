---
title: "PivotItem.IsMissing"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PivotItem. Указывает, был ли элемент удалён из источника данных"
type: docs
url: /ru/net/aspose.cells.pivot/pivotitem/ismissing/
---
## PivotItem.IsMissing property

Указывает, был ли элемент удалён из источника данных.

```csharp
public bool IsMissing { get; }
```

### Примечания

True означает, что это значение было удалено из источника данных.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotItemPropertyIsMissingDemo
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
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int index = pivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];

            // Добавить поле строки
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");

            // Добавить поле данных
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Обновить данные сводной таблицы
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Получить первый элемент сводки в первом поле строки
            PivotField rowField = pivotTable.RowFields[0];
            PivotItem pivotItem = rowField.PivotItems[0];

            // Отобразить значение свойства IsMissing
            Console.WriteLine("IsMissing value for '{0}': {1}", pivotItem.Name, pivotItem.IsMissing);

            // Создать сценарий, в котором элемент может отсутствовать
            worksheet.Cells["A5"].PutValue("Grape");
            worksheet.Cells["B5"].PutValue(4000);
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Проверить, отсутствует ли теперь исходный элемент сводки
            Console.WriteLine("After data change - IsMissing value for '{0}': {1}", 
                pivotItem.Name, pivotItem.IsMissing);

            // Сохраните книгу
            workbook.Save("PivotItemIsMissingDemo.xlsx");
        }
    }
}
```

### См. также

* class [PivotItem](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)



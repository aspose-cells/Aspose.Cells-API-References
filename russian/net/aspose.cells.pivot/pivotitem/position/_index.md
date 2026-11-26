---
title: "PivotItem.Position"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PivotItem. Указывает индекс этого элемента среди всех PivotItem данного поля"
type: docs
url: /ru/net/aspose.cells.pivot/pivotitem/position/
---
## PivotItem.Position property

Указывает индекс этого элемента среди всех PivotItems поля.

```csharp
public int Position { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotItemPropertyPositionDemo
    {
        public static void Run()
        {
            // Создайте книгу с примерными данными
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Добавить примерные данные для сводной таблицы
            sheet.Cells["A1"].PutValue("Product");
            sheet.Cells["B1"].PutValue("Sales");
            sheet.Cells["A2"].PutValue("Apple");
            sheet.Cells["A3"].PutValue("Banana");
            sheet.Cells["A4"].PutValue("Orange");
            sheet.Cells["B2"].PutValue(1000);
            sheet.Cells["B3"].PutValue(2000);
            sheet.Cells["B4"].PutValue(3000);

            // Создать сводную таблицу
            int index = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            
            // Добавить поле строки
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            
            // Добавить поле данных
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Продемонстрируйте свойство Position
            PivotField rowField = pivotTable.RowFields[0];
            foreach (PivotItem item in rowField.PivotItems)
            {
                Console.WriteLine($"Before - Name: {item.Name}, Position: {item.Position}");
                item.Position = 0; // Set position to 0
                Console.WriteLine($"After - Name: {item.Name}, Position: {item.Position}");
            }

            // Обновить и вычислить сводную таблицу
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Сохраните книгу
            workbook.Save("PivotItemPositionDemo.xlsx");
        }
    }
}
```

### См. также

* class [PivotItem](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)



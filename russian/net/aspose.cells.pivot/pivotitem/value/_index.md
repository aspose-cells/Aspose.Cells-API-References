---
title: "PivotItem.Value"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PivotItem. Получает значение элемента сводной таблицы"
type: docs
url: /ru/net/aspose.cells.pivot/pivotitem/value/
---
## PivotItem.Value property

Получает значение элемента сводки

```csharp
public object Value { get; }
```

### Примеры

```csharp
using System;
using System.Collections.Generic;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotItemPropertyValueDemo
    {
        public static void Run()
        {
            // Создайте книгу с примерными данными
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Добавить примерные данные для сводной таблицы
            var cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 15;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 20;
            cells["A5"].Value = "Apple";
            cells["B5"].Value = 5;

            // Создать сводную таблицу
            int index = sheet.PivotTables.Add("A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            
            // Добавить поле строки
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            
            // Добавить поле данных
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");
            
            // Получить поле сводной таблицы
            PivotField pivotField = pivotTable.RowFields[0];
            
            // Обработать элементы сводной таблицы
            List<string> valuesToShow = new List<string> { "Apple", "Banana" };
            
            Console.WriteLine("Pivot Items Before Filtering:");
            PrintPivotItems(pivotField);

            // Отфильтровать элементы сводной таблицы на основе свойства Value
            for (int i = 0; i < pivotField.PivotItems.Count; i++)
            {
                PivotItem item = pivotField.PivotItems[i];
                string itemValue = item.Value?.ToString() ?? "";
                
                if (!valuesToShow.Contains(itemValue))
                {
                    item.IsHidden = true;
                }
            }

            Console.WriteLine("\nPivot Items After Filtering:");
            PrintPivotItems(pivotField);
        }

        private static void PrintPivotItems(PivotField pivotField)
        {
            for (int i = 0; i < pivotField.PivotItems.Count; i++)
            {
                PivotItem item = pivotField.PivotItems[i];
                Console.WriteLine($"Name: {item.Name}, Value: {item.Value}, Hidden: {item.IsHidden}");
            }
        }
    }
}
```

### См. также

* class [PivotItem](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)



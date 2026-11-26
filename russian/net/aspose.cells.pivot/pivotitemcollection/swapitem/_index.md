---
title: "PivotItemCollection.SwapItem"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод PivotItemCollection. Непосредственно меняет местами два элемента"
type: docs
url: /ru/net/aspose.cells.pivot/pivotitemcollection/swapitem/
---
## PivotItemCollection.SwapItem method

Непосредственно меняет местами два элемента.

```csharp
public void SwapItem(int index1, int index2)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| index1 | Int32 |  |
| index2 | Int32 |  |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotItemCollectionMethodSwapItemWithInt32Int32Demo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные для сводной таблицы
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["B3"].Value = 200;
            worksheet.Cells["B4"].Value = 300;

            // Создать сводную таблицу
            int index = worksheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");

            // Получить элементы сводной таблицы
            PivotField pivotField = pivotTable.RowFields[0];
            PivotItemCollection pivotItems = pivotField.PivotItems;

            try
            {
                // Отобразить исходный порядок
                Console.WriteLine("Original order:");
                foreach (PivotItem item in pivotItems)
                {
                    Console.WriteLine(item.Name);
                }

                // Поменять местами элементы с индексами 0 и 1
                pivotItems.SwapItem(0, 1);

                // Отобразить новый порядок
                Console.WriteLine("\nAfter swapping:");
                foreach (PivotItem item in pivotItems)
                {
                    Console.WriteLine(item.Name);
                }

                Console.WriteLine("SwapItem method executed successfully with parameters (0, 1)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SwapItem method: {ex.Message}");
            }

            // Сохранить результат
            workbook.Save("PivotItemCollectionMethodSwapItemWithInt32Int32Demo.xlsx");
        }
    }
}
```

### См. также

* class [PivotItemCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)



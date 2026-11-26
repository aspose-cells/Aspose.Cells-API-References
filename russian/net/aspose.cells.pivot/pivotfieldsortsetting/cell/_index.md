---
title: "PivotFieldSortSetting.Cell"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PivotFieldSortSetting. Сортирует по значениям в строке или столбце"
type: docs
url: /ru/net/aspose.cells.pivot/pivotfieldsortsetting/cell/
---
## PivotFieldSortSetting.Cell property

Сортирует по значениям в строке или столбце.

```csharp
public string Cell { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldSortSettingPropertyCellDemo
    {
        public static void Run()
        {
            // Создайте книгу с примерными данными
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Добавить примерные данные для сводной таблицы
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["A3"].Value = "Orange";
            cells["A4"].Value = "Banana";
            cells["B2"].Value = 10;
            cells["B3"].Value = 5;
            cells["B4"].Value = 8;

            // Создать сводную таблицу
            int index = sheet.PivotTables.Add("A1:B4", "D3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Сортировать по ссылке на ячейку
            pivotTable.RowFields[0].SortBy(SortOrder.Ascending, 0, PivotLineType.Regular, "A2");
            
            // Продемонстрировать использование свойства Cell
            Console.WriteLine("Sorting by cell: " + pivotTable.RowFields[0].SortSetting.Cell);
            
            // Изменить ячейку сортировки
            pivotTable.RowFields[0].SortBy(SortOrder.Ascending, 0, PivotLineType.Regular, "A3");
            Console.WriteLine("Changed sort cell to: " + pivotTable.RowFields[0].SortSetting.Cell);
            
            // Очистить сортировку ячеек
            pivotTable.RowFields[0].SortBy(SortOrder.Ascending, 0, PivotLineType.GrandTotal, "");
            Console.WriteLine("After clearing cell sort: " + 
                (string.IsNullOrEmpty(pivotTable.RowFields[0].SortSetting.Cell) ? "Empty" : "Has value"));
        }
    }
}
```

### См. также

* class [PivotFieldSortSetting](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)



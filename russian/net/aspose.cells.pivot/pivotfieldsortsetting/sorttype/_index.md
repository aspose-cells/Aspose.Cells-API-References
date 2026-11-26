---
title: "PivotFieldSortSetting.SortType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PivotFieldSortSetting. Представляет SortOrder"
type: docs
url: /ru/net/aspose.cells.pivot/pivotfieldsortsetting/sorttype/
---
## PivotFieldSortSetting.SortType property

Представляет [`SortOrder`](../../../aspose.cells/sortorder/).

```csharp
public SortOrder SortType { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldSortSettingPropertySortTypeDemo
    {
        public static void Run()
        {
            // Создайте книгу с примерными данными
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
            worksheet.Cells["B4"].Value = 150;

            // Создать сводную таблицу
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Добавить поле строки
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            
            // Отсортировать поле строки по возрастанию
            pivotTable.RowFields[0].SortBy(SortOrder.Ascending, 0, PivotLineType.Regular, "E5");
            
            // Продемонстрировать свойство SortType
            Console.WriteLine("Sort Type: " + pivotTable.RowFields[0].SortSetting.SortType);
            Console.WriteLine("Sorted by cell: " + pivotTable.RowFields[0].SortSetting.Cell);
            
            // Изменить порядок сортировки и продемонстрировать снова
            pivotTable.RowFields[0].SortBy(SortOrder.Descending, 0, PivotLineType.Regular, "E6");
            Console.WriteLine("Updated Sort Type: " + pivotTable.RowFields[0].SortSetting.SortType);
            Console.WriteLine("Updated sorted by cell: " + pivotTable.RowFields[0].SortSetting.Cell);
        }
    }
}
```

### См. также

* enum [SortOrder](../../../aspose.cells/sortorder/)
* class [PivotFieldSortSetting](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)



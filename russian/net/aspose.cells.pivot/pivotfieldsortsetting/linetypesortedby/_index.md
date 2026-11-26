---
title: "PivotFieldSortSetting.LineTypeSortedBy"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PivotFieldSortSetting. Тип линии сводной таблицы, по которому выполнена сортировка"
type: docs
url: /ru/net/aspose.cells.pivot/pivotfieldsortsetting/linetypesortedby/
---
## PivotFieldSortSetting.LineTypeSortedBy property

Тип строки сводной таблицы, по которому выполнена сортировка.

```csharp
public PivotLineType LineTypeSortedBy { get; }
```

### Примечания

Работает только когда это поле не сортируется по меткам.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldSortSettingPropertyLineTypeSortedByDemo
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
            cells["B3"].Value = 15;
            cells["B4"].Value = 5;

            // Создать сводную таблицу
            int index = sheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            
            // Добавить поле строки
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            
            // Сортировать по возрастанию с типом линии — передайте пустую строку для параметра cellName
            pivotTable.RowFields[0].SortBy(SortOrder.Ascending, 0, PivotLineType.GrandTotal, "");
            
            // Продемонстрировать свойство LineTypeSortedBy
            Console.WriteLine("LineTypeSortedBy: " + pivotTable.RowFields[0].SortSetting.LineTypeSortedBy);
            
            // Изменить сортировку, чтобы использовать обычный тип строки
            pivotTable.RowFields[0].SortBy(SortOrder.Descending, 0, PivotLineType.Regular, "C5");
            Console.WriteLine("LineTypeSortedBy after change: " + pivotTable.RowFields[0].SortSetting.LineTypeSortedBy);
        }
    }
}
```

### См. также

* enum [PivotLineType](../../pivotlinetype/)
* class [PivotFieldSortSetting](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)



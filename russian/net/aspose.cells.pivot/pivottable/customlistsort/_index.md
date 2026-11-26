---
title: "PivotTable.CustomListSort"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PivotTable. Указывает, следует ли учитывать встроенный пользовательский список при сортировке данных"
type: docs
url: /ru/net/aspose.cells.pivot/pivottable/customlistsort/
---
## PivotTable.CustomListSort property

Указывает, следует ли учитывать встроенный пользовательский список при сортировке данных

```csharp
public bool CustomListSort { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyCustomListSortDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Добавить примерные данные для сводной таблицы
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 20;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 15;
            cells["A5"].Value = "Pear";
            cells["B5"].Value = 5;

            // Создать сводную таблицу
            int index = sheet.PivotTables.Add("A1:B5", "C3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];

            // Добавить поле строки и поле данных
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");

            // Включить сортировку пользовательского списка
            pivotTable.CustomListSort = true;

            // Сохраните книгу
            workbook.Save("PivotTable_CustomListSort_Example.xlsx");
        }
    }
}
```

### См. также

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)



---
title: "PivotTable.Tag"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PivotTable. Получает и задает пользовательскую строку, связанную с этим представлением сводной таблицы"
type: docs
url: /ru/net/aspose.cells.pivot/pivottable/tag/
---
## PivotTable.Tag property

Получает и задает пользовательскую строку, связанную с этим представлением PivotTable.

```csharp
public string Tag { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyTagDemo
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
            cells["B3"].Value = 15;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 20;

            // Создать сводную таблицу
            PivotTableCollection pivotTables = sheet.PivotTables;
            int index = pivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];

            // Добавить поля в сводную таблицу
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");

            // Установить и продемонстрировать свойство Tag
            pivotTable.Tag = "SamplePivotTableTag";
            Console.WriteLine("Pivot Table Tag: " + pivotTable.Tag);

            // Сохраните книгу
            workbook.Save("PivotTableTagDemo.xlsx");
        }
    }
}
```

### См. также

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)



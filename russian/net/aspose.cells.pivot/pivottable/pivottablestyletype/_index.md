---
title: "PivotTable.PivotTableStyleType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PivotTable. Получает и задает встроенный стиль сводной таблицы"
type: docs
url: /ru/net/aspose.cells.pivot/pivottable/pivottablestyletype/
---
## PivotTable.PivotTableStyleType property

Получает и задаёт встроенный стиль сводной таблицы.

```csharp
public PivotTableStyleType PivotTableStyleType { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyPivotTableStyleTypeDemo
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
            cells["B3"].Value = 5;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 7;

            // Создать сводную таблицу
            int index = sheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];

            // Установить и продемонстрировать PivotTableStyleType
            pivotTable.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;
            Console.WriteLine("PivotTable Style Type: " + pivotTable.PivotTableStyleType);

            // Сохраните книгу
            workbook.Save("PivotTableStyleTypeDemo.xlsx");
        }
    }
}
```

### См. также

* enum [PivotTableStyleType](../../pivottablestyletype/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)



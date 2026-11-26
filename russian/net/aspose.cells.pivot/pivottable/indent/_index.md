---
title: "PivotTable.Indent"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PivotTable. Указывает шаг отступа для компактной оси и может использоваться для установки макета отчёта в компактную форму"
type: docs
url: /ru/net/aspose.cells.pivot/pivottable/indent/
---
## PivotTable.Indent property

Задает шаг отступа для компактной оси и может использоваться для установки макета отчёта в компактную форму.

```csharp
public int Indent { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyIndentDemo
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

            // Установить свойство отступа
            pivotTable.Indent = 3;
            Console.WriteLine("Pivot Table Indent: " + pivotTable.Indent);

            // Сохраните книгу
            workbook.Save("PivotTableIndentDemo.xlsx");
        }
    }
}
```

### См. также

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)



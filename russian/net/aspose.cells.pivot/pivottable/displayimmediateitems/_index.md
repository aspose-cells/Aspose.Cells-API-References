---
title: "PivotTable.DisplayImmediateItems"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PivotTable. Указывает, видимы ли элементы в областях строк и столбцов, когда область данных PivotTable пуста. Значение по умолчанию — true."
type: docs
url: /ru/net/aspose.cells.pivot/pivottable/displayimmediateitems/
---
## PivotTable.DisplayImmediateItems property

Указывает, видимы ли элементы в областях строк и столбцов, когда область данных PivotTable пуста. Значение по умолчанию — true.

```csharp
public bool DisplayImmediateItems { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyDisplayImmediateItemsDemo
    {
        public static void Run()
        {
            // Создать книгу
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
            int pivotIndex = sheet.PivotTables.Add("A1:B4", "D1", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];

            // Добавить поля в сводную таблицу
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");

            // Продемонстрировать свойство DisplayImmediateItems
            Console.WriteLine("Initial DisplayImmediateItems value: " + pivotTable.DisplayImmediateItems);
            
            // Изменить значение свойства
            pivotTable.DisplayImmediateItems = false;
            Console.WriteLine("After setting to false: " + pivotTable.DisplayImmediateItems);

            // Сохраните книгу
            workbook.Save("PivotTableDisplayImmediateItemsDemo.xlsx");
        }
    }
}
```

### См. также

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)



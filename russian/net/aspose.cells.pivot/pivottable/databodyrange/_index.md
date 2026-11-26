---
title: "PivotTable.DataBodyRange"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PivotTable. Возвращает объект CellArea, представляющий диапазон, содержащий область данных в списке между строкой заголовка и строкой вставки. Только для чтения"
type: docs
url: /ru/net/aspose.cells.pivot/pivottable/databodyrange/
---
## PivotTable.DataBodyRange property

Возвращает объект [`CellArea`](../../../aspose.cells/cellarea/), представляющий диапазон, содержащий область данных в списке между строкой заголовка и строкой вставки. Только для чтения.

```csharp
public CellArea DataBodyRange { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyDataBodyRangeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            Cells cells = sheet.Cells;

            // Добавить примерные данные для сводной таблицы
            cells["A1"].Value = "Product";
            cells["B1"].Value = "Sales";
            cells["A2"].Value = "Bike";
            cells["B2"].Value = 1000;
            cells["A3"].Value = "Car";
            cells["B3"].Value = 2000;
            cells["A4"].Value = "Bike";
            cells["B4"].Value = 1500;
            cells["A5"].Value = "Car";
            cells["B5"].Value = 2500;

            // Добавьте сводную таблицу
            int pivotIndex = sheet.PivotTables.Add("A7", "A1:B5", "PivotTable1");
            PivotTable pivot = sheet.PivotTables[pivotIndex];
            
            // Настройте сводную таблицу
            pivot.AddFieldToArea(PivotFieldType.Row, "Product");
            pivot.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Обновить данные сводной таблицы
            pivot.RefreshData();
            pivot.CalculateData();

            // Продемонстрировать использование DataBodyRange
            CellArea dataBodyArea = pivot.DataBodyRange;
            Console.WriteLine($"Data body range: StartRow={dataBodyArea.StartRow}, EndRow={dataBodyArea.EndRow}, StartColumn={dataBodyArea.StartColumn}, EndColumn={dataBodyArea.EndColumn}");

            // Сохраните книгу
            workbook.Save("PivotTableDataBodyRangeDemo.xlsx");
        }
    }
}
```

### См. также

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)



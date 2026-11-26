---
title: "PivotTable.RowRange"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PivotTable. Возвращает объект CellArea, представляющий диапазон, содержащий строковую область в отчете сводной таблицы. Только для чтения"
type: docs
url: /ru/net/aspose.cells.pivot/pivottable/rowrange/
---
## PivotTable.RowRange property

Возвращает объект CellArea, представляющий диапазон, содержащий область строк в отчёте PivotTable. Только для чтения.

```csharp
public CellArea RowRange { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyRowRangeDemo
    {
        public static void Run()
        {
            // Создать книгу из исходного файла Excel
            Workbook workbook = new Workbook("example.xlsx");
            
            // Обновить все сводные таблицы в книге
            workbook.Worksheets.RefreshAll();
            
            // Получите первую сводную таблицу с первого листа
            PivotTable pivotTable = workbook.Worksheets[0].PivotTables[0];
            
            // Получите диапазон строк сводной таблицы
            CellArea rowRange = pivotTable.RowRange;
            
            // Отобразите координаты диапазона строк
            Console.WriteLine("PivotTable Row Range:");
            Console.WriteLine($"Start Row: {rowRange.StartRow}");
            Console.WriteLine($"End Row: {rowRange.EndRow}");
            Console.WriteLine($"Start Column: {rowRange.StartColumn}");
            Console.WriteLine($"End Column: {rowRange.EndColumn}");
            
            // Получите диапазон столбцов сводной таблицы
            CellArea columnRange = pivotTable.ColumnRange;
            
            // Отобразите координаты диапазона столбцов
            Console.WriteLine("\nPivotTable Column Range:");
            Console.WriteLine($"Start Row: {columnRange.StartRow}");
            Console.WriteLine($"End Row: {columnRange.EndRow}");
            Console.WriteLine($"Start Column: {columnRange.StartColumn}");
            Console.WriteLine($"End Column: {columnRange.EndColumn}");
        }
    }
}
```

### См. также

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)



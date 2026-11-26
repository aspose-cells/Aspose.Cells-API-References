---
title: "Cells.Rows"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Cells. Возвращает коллекцию объектов Row, представляющих отдельные строки в этом листе"
type: docs
url: /ru/net/aspose.cells/cells/rows/
---
## Cells.Rows property

Возвращает коллекцию объектов [`Row`](../../row/) , представляющих отдельные строки в этом листе.

```csharp
public RowCollection Rows { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyRowsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Установите ширину столбца и высоту строки
            worksheet.Cells.SetColumnWidthPixel(0, 200);
            worksheet.Cells.Rows[0].Height = 50;
            
            // Получите доступ к свойствам строки через коллекцию Rows
            Row row = worksheet.Cells.Rows[0];
            Console.WriteLine($"Row 0 height: {row.Height}");
            Console.WriteLine($"Is height matched: {row.IsHeightMatched}");
            
            // Измените свойства строки
            row.IsHeightMatched = true;
            row.Height = 60;
            
            // Проверьте изменения
            Console.WriteLine($"Modified row 0 height: {worksheet.Cells.GetRowHeightPixel(0)}");
            Console.WriteLine($"Is height matched after change: {row.IsHeightMatched}");
            
            // Сохраните книгу
            workbook.Save("CellsPropertyRowsDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### См. также

* class [RowCollection](../../rowcollection/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



---
title: "Cells.MaxDataRow"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Cells. Максимальный индекс строки ячейки, содержащей данные"
type: docs
url: /ru/net/aspose.cells/cells/maxdatarow/
---
## Cells.MaxDataRow property

Максимальный индекс строки ячейки, содержащей данные.

```csharp
public int MaxDataRow { get; }
```

### Примечания

Возвращает -1, если нет ячейки, содержащей данные. Это свойство требует итерации и динамической проверки ячеек и строк, поэтому является ресурсоёмким процессом и не должно вызываться многократно, например, использовать его напрямую в условии цикла.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyMaxDataRowDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            sheet.Cells["A1"].PutValue("Name");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["A2"].PutValue("Item1");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["A3"].PutValue("Item2");
            sheet.Cells["B3"].PutValue(20);
            sheet.Cells["A4"].PutValue("Item3");
            sheet.Cells["B4"].PutValue(30);

            // Продемонстрировать использование MaxDataRow
            int maxRow = sheet.Cells.MaxDataRow;
            Console.WriteLine("Max data row: " + maxRow);

            // Создайте область ячеек, используя MaxDataRow
            int startRow = 0;
            int startColumn = 0;
            int endRow = sheet.Cells.MaxDataRow;
            int endColumn = sheet.Cells.MaxDataColumn;

            // Применить форматирование к диапазону данных
            Style style = workbook.CreateStyle();
            style.Font.IsBold = true;
            
            // Примените стиль к диапазону
            sheet.Cells.CreateRange(startRow, startColumn, endRow + 1, endColumn + 1).ApplyStyle(style, new StyleFlag { FontBold = true });

            // Сохраните книгу
            workbook.Save("MaxDataRowDemo.xlsx");
        }
    }
}
```

### См. также

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



---
title: "Row.GetStyle"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Row. Получает стиль этой строки"
type: docs
url: /ru/net/aspose.cells/row/getstyle/
---
## Row.GetStyle method

Получает стиль этой строки.

```csharp
public Style GetStyle()
```

### Примечания

Изменение возвращённого объекта стиля напрямую не оказывает влияния на эту строку или любые ячейки в ней. Вам необходимо вызвать метод [`ApplyStyle`](../applystyle/) или [`SetStyle`](../setstyle/), чтобы применить изменение к этой строке. Стиль строки — это стиль, который будет наследоваться ячейками в этой строке (те ячейки, у которых нет пользовательских настроек стиля, такие как существующие ячейки, для которых стиль не был установлен явно, или те, которые ещё не созданы).

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowMethodGetStyleDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Установить стили для демонстрации
            Style rowStyle = workbook.CreateStyle();
            rowStyle.Pattern = BackgroundType.Solid;
            rowStyle.ForegroundColor = System.Drawing.Color.Blue;
            cells.Rows[8].ApplyStyle(rowStyle, new StyleFlag { All = true });

            Style columnStyle = workbook.CreateStyle();
            columnStyle.Pattern = BackgroundType.Solid;
            columnStyle.ForegroundColor = System.Drawing.Color.Red;
            cells.Columns[5].ApplyStyle(columnStyle, new StyleFlag { All = true });

            // Продемонстрировать использование GetStyle
            Style retrievedRowStyle = cells.Rows[8].GetStyle();
            Console.WriteLine("Row 8 Style - ForegroundColor: " + retrievedRowStyle.ForegroundColor);
            Console.WriteLine("Row 8 Style - Pattern: " + retrievedRowStyle.Pattern);

            Style retrievedColumnStyle = cells.Columns[5].GetStyle();
            Console.WriteLine("Column 5 Style - ForegroundColor: " + retrievedColumnStyle.ForegroundColor);
            Console.WriteLine("Column 5 Style - Pattern: " + retrievedColumnStyle.Pattern);
        }
    }
}
```

### См. также

* class [Style](../../style/)
* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



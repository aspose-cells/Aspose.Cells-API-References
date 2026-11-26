---
title: "Column.GetStyle"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Column. Получает стиль этой колонки"
type: docs
url: /ru/net/aspose.cells/column/getstyle/
---
## Column.GetStyle method

Получает стиль этого столбца.

```csharp
public Style GetStyle()
```

### Примечания

Изменение возвращённого объекта стиля напрямую не оказывает влияния на эту колонку или любые ячейки в этой колонке. Вам необходимо вызвать метод [`ApplyStyle`](../applystyle/) или [`SetStyle`](../setstyle/), чтобы применить изменение к этой колонке. Стиль колонки — это стиль, который будет наследоваться ячейками в этой колонке (те ячейки, у которых нет пользовательских настроек стиля, такие как существующие ячейки, для которых стиль не был установлен явно, или те, которые ещё не созданы)

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ColumnMethodGetStyleDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Установите стиль для столбца 5
            Style columnStyle = cells.Columns[5].GetStyle();
            columnStyle.Font.Name = "Arial";
            columnStyle.Font.Size = 14;
            columnStyle.Font.IsBold = true;
            cells.Columns[5].ApplyStyle(columnStyle, new StyleFlag { Font = true });

            // Установите стиль для строки 7
            Style rowStyle = cells.Rows[7].GetStyle();
            rowStyle.Font.Color = System.Drawing.Color.Red;
            rowStyle.Font.IsItalic = true;
            cells.Rows[7].ApplyStyle(rowStyle, new StyleFlag { Font = true });

            // Проверьте стиль колонки
            Style retrievedColumnStyle = cells.Columns[5].GetStyle();
            Console.WriteLine("Column 5 Style:");
            Console.WriteLine($"Font: {retrievedColumnStyle.Font.Name}, Size: {retrievedColumnStyle.Font.Size}, Bold: {retrievedColumnStyle.Font.IsBold}");

            // Проверьте стиль строки
            Style retrievedRowStyle = cells.Rows[7].GetStyle();
            Console.WriteLine("\nRow 7 Style:");
            Console.WriteLine($"Color: {retrievedRowStyle.Font.Color}, Italic: {retrievedRowStyle.Font.IsItalic}");

            // Сохраните книгу
            workbook.Save("ColumnMethodGetStyleDemo_output.xlsx");
        }
    }
}
```

### См. также

* class [Style](../../style/)
* class [Column](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



---
title: "Column.Width"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Column. Получает и задает ширину колонки в единицах символов"
type: docs
url: /ru/net/aspose.cells/column/width/
---
## Column.Width property

Получает и задает ширину столбца в символах.

```csharp
public double Width { get; set; }
```

### Примечания

Для электронных таблиц ширина столбца измеряется количеством символов максимальной ширины цифр чисел 0~9, отображаемых шрифтом обычного стиля.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ColumnPropertyWidthDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Установить ширину для колонки 3 (индекс 2)
            worksheet.Cells.Columns[2].Width = 25.5;
            
            // Установить ширину для колонки 4 (индекс 3)
            worksheet.Cells.Columns[3].Width = 40.0;
            
            // Получить и отобразить ширины
            Console.WriteLine("Column 3 Width: " + worksheet.Cells.Columns[2].Width);
            Console.WriteLine("Column 4 Width: " + worksheet.Cells.Columns[3].Width);
            
            // Сохраните книгу
            workbook.Save("ColumnWidthDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### См. также

* class [Column](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



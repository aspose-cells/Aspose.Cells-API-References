---
title: "StyleFlag.LeftBorder"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство StyleFlag. Параметры левой границы будут применены"
type: docs
url: /ru/net/aspose.cells/styleflag/leftborder/
---
## StyleFlag.LeftBorder property

Настройки левой границы будут применены.

```csharp
public bool LeftBorder { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class StyleFlagPropertyLeftBorderDemo
    {
        public static void Run()
        {
            // Создать книгу
            var workbook = new Workbook();
            var worksheet = workbook.Worksheets[0];

            // Создайте диапазон и примените стиль левой границы
            var range = worksheet.Cells.CreateRange(1, 1, 1, 1);
            range.PutValue("Left Border Demo", false, false);

            // Создайте стиль и флаг
            var style = workbook.CreateStyle();
            var flag = new StyleFlag();

            // Установите свойства левой границы
            style.Borders[BorderType.LeftBorder].Color = Color.Green;
            style.Borders[BorderType.LeftBorder].LineStyle = CellBorderType.Thick;
            flag.LeftBorder = true;

            // Примените стиль с флагом левой границы
            range.ApplyStyle(style, flag);

            // Проверьте, что левая граница была применена
            var appliedStyle = worksheet.Cells[1, 1].GetStyle();
            Console.WriteLine($"Left border color: {appliedStyle.Borders[BorderType.LeftBorder].Color}");
            Console.WriteLine($"Left border style: {appliedStyle.Borders[BorderType.LeftBorder].LineStyle}");

            // Сохраните книгу
            workbook.Save("LeftBorderDemo.xlsx");
        }
    }
}
```

### См. также

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



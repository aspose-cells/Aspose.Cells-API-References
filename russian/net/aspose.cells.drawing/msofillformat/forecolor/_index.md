---
title: "MsoFillFormat.ForeColor"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство MsoFillFormat. Получает и задает передний цвет заливки"
type: docs
url: /ru/net/aspose.cells.drawing/msofillformat/forecolor/
---
## MsoFillFormat.ForeColor property

Получает и задает основной цвет заливки.

```csharp
public Color ForeColor { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class MsoFillFormatPropertyForeColorDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте прямоугольную форму со всеми необходимыми параметрами
            var rectangle = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 150, 200);

            // Получить формат заливки
            MsoFillFormat fillFormat = rectangle.FillFormat;

            // Установить и продемонстрировать свойство ForeColor
            fillFormat.ForeColor = System.Drawing.Color.Red;
            Console.WriteLine("ForeColor set to: " + fillFormat.ForeColor);

            // Изменить ForeColor
            fillFormat.ForeColor = System.Drawing.Color.FromArgb(0, 128, 255);
            Console.WriteLine("ForeColor changed to: " + fillFormat.ForeColor);

            // Сохраните книгу
            workbook.Save("MsoFillFormatForeColorDemo.xlsx");
        }
    }
}
```

### См. также

* class [MsoFillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)



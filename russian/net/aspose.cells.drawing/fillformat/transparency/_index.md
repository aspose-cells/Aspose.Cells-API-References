---
title: "FillFormat.Transparency"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство FillFormat. Возвращает или задает степень прозрачности области значением от 0.0 (непрозрачный) до 1.0 (полностью прозрачный)"
type: docs
url: /ru/net/aspose.cells.drawing/fillformat/transparency/
---
## FillFormat.Transparency property

Возвращает или задает степень прозрачности области значением от 0.0 (непрозрачный) до 1.0 (прозрачный).

```csharp
public double Transparency { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class FillFormatPropertyTransparencyDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить фигуру для демонстрации прозрачности
            Shape shape = worksheet.Shapes.AddRectangle(10, 10, 200, 100, 50, 50);

            // Установить свойства заполнения с прозрачностью
            shape.Fill.FillType = FillType.Solid;
            shape.Fill.SolidFill.Color = System.Drawing.Color.Blue;
            shape.Fill.Transparency = 0.3; // 30% transparent

            // Сохраните книгу
            workbook.Save("FillFormatTransparencyDemo.xlsx");
        }
    }
}
```

### См. также

* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)



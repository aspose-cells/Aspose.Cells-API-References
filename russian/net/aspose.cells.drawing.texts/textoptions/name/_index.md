---
title: "TextOptions.Name"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство TextOptions. Получает и задает имя фигуры"
type: docs
url: /ru/net/aspose.cells.drawing.texts/textoptions/name/
---
## TextOptions.Name property

Получает и задает имя фигуры.

```csharp
public override string Name { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class TextOptionsPropertyNameDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            Shape shape = sheet.Shapes.AddAutoShape(AutoShapeType.Rectangle, 10, 10, 200, 100, 0, 0);
            shape.Text = "Sample Text";
            
            FontSetting fontSetting = shape.Characters(0, shape.Text.Length);
            TextOptions textOptions = fontSetting.TextOptions;
            
            // Продемонстрировать использование свойства Name
            textOptions.Name = "Arial";
            textOptions.Size = 14;
            textOptions.IsBold = true;
            textOptions.Color = System.Drawing.Color.Blue;
            
            workbook.Save("TextOptionsPropertyNameDemo.xlsx");
        }
    }
}
```

### См. также

* class [TextOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)



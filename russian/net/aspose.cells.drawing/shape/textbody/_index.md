---
title: "Shape.TextBody"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Shape. Получает и задает настройку текста формы"
type: docs
url: /ru/net/aspose.cells.drawing/shape/textbody/
---
## Shape.TextBody property

Получает и задает настройку текста фигуры.

```csharp
public FontSettingCollection TextBody { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class ShapePropertyTextBodyDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 200);
            FontSettingCollection fontSettingCollection = shape.TextBody;
            fontSettingCollection.Text = "This is a test.";

            workbook.Save("ShapeTextBodyDemo.xlsx");
        }
    }
}
```

### См. также

* class [FontSettingCollection](../../../aspose.cells.drawing.texts/fontsettingcollection/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)



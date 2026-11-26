---
title: "Shape.Hyperlink"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Shape. Получает гиперссылку фигуры"
type: docs
url: /ru/net/aspose.cells.drawing/shape/hyperlink/
---
## Shape.Hyperlink property

Получает гиперссылку фигуры.

```csharp
public Hyperlink Hyperlink { get; }
```

### Примеры

```csharp
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ShapePropertyHyperlinkDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            Aspose.Cells.Drawing.Shape shape = sheet.Shapes.AddRectangle(0, 0, 10, 10, 100, 150);
            Hyperlink hyperlink = shape.Hyperlink;
            hyperlink.Address = "https://www.aspose.com";
            hyperlink.ScreenTip = "Click to open Aspose website";

            workbook.Save("ShapeHyperlinkDemo.xlsx");
        }
    }
}
```

### См. также

* class [Hyperlink](../../../aspose.cells/hyperlink/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)



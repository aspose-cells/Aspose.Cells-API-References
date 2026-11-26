---
title: "MsoFillFormat.BackColor"
second_title: "Справочник API Aspose.Cells для .NET"
description: "MsoFillFormat property. Получает и задает цвет фона"
type: docs
url: /ru/net/aspose.cells.drawing/msofillformat/backcolor/
---
## MsoFillFormat.BackColor property

Получает и задает цвет фона файла.

```csharp
public Color BackColor { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class MsoFillFormatPropertyBackColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            ArcShape arcShape = worksheet.Shapes.AddArc(2, 0, 2, 0, 130, 130);
            MsoFillFormat fillFormat = arcShape.FillFormat;

            fillFormat.ForeColor = Color.Blue;
            fillFormat.BackColor = Color.LightBlue;
            fillFormat.Transparency = 0.5;

            Console.WriteLine("BackColor set to: " + fillFormat.BackColor.Name);

            workbook.Save("MsoFillFormatBackColorDemo.xlsx");
        }
    }
}
```

### См. также

* class [MsoFillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)



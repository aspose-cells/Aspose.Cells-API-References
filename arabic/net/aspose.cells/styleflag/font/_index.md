---
title: "StyleFlag.Font"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية StyleFlag. سيتم تطبيق إعدادات الخط"
type: docs
url: /ar/net/aspose.cells/styleflag/font/
---
## StyleFlag.Font property

سيتم تطبيق إعدادات الخط.

```csharp
public bool Font { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class StyleFlagPropertyFontDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            var shape = workbook.Worksheets[0].Shapes.AddButton(0, 0, 100, 100, 100, 100);
            shape.Text = "Sample Text";
            
            Aspose.Cells.Font font = workbook.CreateStyle().Font;
            font.Name = "Arial";
            font.Size = 14;
            font.Color = Color.Blue;
            font.IsBold = true;
            
            StyleFlag flag = new StyleFlag();
            flag.Font = true;
            
            shape.FormatCharacters(0, shape.Text.Length, font, flag);
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



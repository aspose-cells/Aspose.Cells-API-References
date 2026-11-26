---
title: "FillFormat.GradientVariant"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство FillFormat. Возвращает вариант градиента для указанного заполнения. Применяется только в Excel 2007"
type: docs
url: /ru/net/aspose.cells.drawing/fillformat/gradientvariant/
---
## FillFormat.GradientVariant property

Возвращает вариант градиента для указанного заполнения. Применяется только для Excel 2007.

```csharp
public int GradientVariant { get; }
```

### Примечания

Может принимать только значение от 1 до 4, соответствующее одному из четырёх вариантов на вкладке Gradient в диалоговом окне Fill Effects. Если стиль равен GradientStyle.FromCenter, аргумент Variant может быть только 1 или 2.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class FillFormatPropertyGradientVariantDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            Shape rectangle = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 200, 150);
            FillFormat fillFormat = rectangle.Fill;
            
            fillFormat.SetTwoColorGradient(Color.LightBlue, Color.DarkBlue, GradientStyleType.Horizontal, 2);
            Console.WriteLine("GradientVariant after SetTwoColorGradient: " + fillFormat.GradientVariant);
            
            fillFormat.SetPresetColorGradient(GradientPresetType.Gold, GradientStyleType.FromCorner, 4);
            Console.WriteLine("GradientVariant after SetPresetColorGradient: " + fillFormat.GradientVariant);
        }
    }
}
```

### См. также

* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)



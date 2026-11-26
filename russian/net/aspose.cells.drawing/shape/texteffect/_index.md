---
title: "Shape.TextEffect"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Shape. Возвращает объект TextEffectFormat, который содержит свойства форматирования текстового эффекта для указанной фигуры. Применяется к объектам Shape, представляющим WordArt"
type: docs
url: /ru/net/aspose.cells.drawing/shape/texteffect/
---
## Shape.TextEffect property

Возвращает объект TextEffectFormat, который содержит свойства форматирования текстовых эффектов для указанной фигуры. Применяется к объектам Shape, представляющим WordArt.

```csharp
public TextEffectFormat TextEffect { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyTextEffectDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте форму WordArt с правильными параметрами
            Shape shape = worksheet.Shapes.AddWordArt(PresetWordArtStyle.WordArtStyle1, "Sample Text", 10, 10, 200, 50, 0, 0);

            // Проверьте, является ли она WordArt, и получите доступ к свойствам TextEffect
            if (shape.IsWordArt)
            {
                TextEffectFormat textEffectFormat = shape.TextEffect;
                textEffectFormat.FontBold = true;
                textEffectFormat.FontItalic = true;
                textEffectFormat.FontName = "Arial";
                textEffectFormat.FontSize = 14;
            }

            // Сохраните книгу
            workbook.Save("TextEffectDemo.xlsx");
        }
    }
}
```

### См. также

* class [TextEffectFormat](../../texteffectformat/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)



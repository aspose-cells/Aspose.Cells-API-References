---
title: "Класс TextEffectFormat"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Drawing.TextEffectFormat. Содержит свойства и методы, применимые к объектам WordArt"
type: docs
url: /ru/net/aspose.cells.drawing/texteffectformat/
---
## TextEffectFormat class

Содержит свойства и методы, применимые к объектам WordArt.

```csharp
public class TextEffectFormat
```

## Свойства

| Имя | Описание |
| --- | --- |
| [FontBold](../../aspose.cells.drawing/texteffectformat/fontbold/) { get; set; } | Указывает, является ли шрифт полужирным. |
| [FontItalic](../../aspose.cells.drawing/texteffectformat/fontitalic/) { get; set; } | Указывает, является ли шрифт курсивом. |
| [FontName](../../aspose.cells.drawing/texteffectformat/fontname/) { get; set; } | Имя шрифта, используемого в WordArt. |
| [FontSize](../../aspose.cells.drawing/texteffectformat/fontsize/) { get; set; } | Размер (в пунктах) шрифта, используемого в WordArt. |
| [PresetShape](../../aspose.cells.drawing/texteffectformat/presetshape/) { get; set; } | Получает и задает предустановленный тип формы. |
| [RotatedChars](../../aspose.cells.drawing/texteffectformat/rotatedchars/) { get; set; } | Если true, символы в указанном WordArt вращаются на 90 градусов относительно ограничивающей формы WordArt. |
| [Text](../../aspose.cells.drawing/texteffectformat/text/) { get; set; } | Текст в WordArt. |

## Методы

| Имя | Описание |
| --- | --- |
| [SetTextEffect](../../aspose.cells.drawing/texteffectformat/settexteffect/)(MsoPresetTextEffect) | Устанавливает предустановленный текстовый эффект. |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassTextEffectFormatDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            ShapeCollection shapes = workbook.Worksheets[0].Shapes;
            
            // Добавить форму текстового эффекта
            shapes.AddTextEffect(MsoPresetTextEffect.TextEffect1, "Aspose", "Arial", 30, false, false, 0, 0, 0, 0, 100, 200);
            
            // Изменить текстовый эффект
            TextEffectFormat textEffectFormat = shapes[0].TextEffect;
            textEffectFormat.SetTextEffect(MsoPresetTextEffect.TextEffect10);
            
            // Сохраните книгу
            workbook.Save("TextEffectDemo.xlsx");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)



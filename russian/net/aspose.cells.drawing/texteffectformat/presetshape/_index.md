---
title: "TextEffectFormat.PresetShape"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство TextEffectFormat. Получает и задает тип предустановленной формы"
type: docs
url: /ru/net/aspose.cells.drawing/texteffectformat/presetshape/
---
## TextEffectFormat.PresetShape property

Получает и задает предустановленный тип формы.

```csharp
public MsoPresetTextEffectShape PresetShape { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TextEffectFormatPropertyPresetShapeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить форму с текстовым эффектом
            Shape shape = worksheet.Shapes.AddTextEffect(
                MsoPresetTextEffect.TextEffect1,
                "Sample Text",
                "Arial",
                18,
                false,
                false,
                0,
                0,
                100,
                200,
                0,
                0);

            // Получить формат текстового эффекта
            TextEffectFormat textEffectFormat = shape.TextEffect;

            // Установить и получить свойство PresetShape
            textEffectFormat.PresetShape = MsoPresetTextEffectShape.ArchUpPour;
            Console.WriteLine("PresetShape: " + textEffectFormat.PresetShape);

            // Изменить другие свойства
            textEffectFormat.Text = "Updated Text";
            textEffectFormat.FontBold = true;
            textEffectFormat.FontSize = 24;

            // Сохраните книгу
            workbook.Save("TextEffectFormatDemo.xlsx");
        }
    }
}
```

### См. также

* enum [MsoPresetTextEffectShape](../../msopresettexteffectshape/)
* class [TextEffectFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)



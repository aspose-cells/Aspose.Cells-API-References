---
title: "TextEffectFormat.SetTextEffect"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод TextEffectFormat. Устанавливает предустановленный текстовый эффект"
type: docs
url: /ru/net/aspose.cells.drawing/texteffectformat/settexteffect/
---
## TextEffectFormat.SetTextEffect method

Устанавливает предустановленный текстовый эффект.

```csharp
public void SetTextEffect(MsoPresetTextEffect effect)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| эффект | MsoPresetTextEffect | Предустановленный текстовый эффект. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class TextEffectFormatMethodSetTextEffectWithMsoPresetTextEffectDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить форму для WordArt
            Shape wordArt = worksheet.Shapes.AddTextEffect(MsoPresetTextEffect.TextEffect1, "Sample Text", "Arial", 36, false, false, 0, 0, 0, 0, 100, 100);

            // Получить TextEffectFormat формы
            TextEffectFormat textEffectFormat = wordArt.TextEffect;

            try
            {
                // Вызвать метод SetTextEffect с параметром MsoPresetTextEffect
                textEffectFormat.SetTextEffect(MsoPresetTextEffect.TextEffect10);

                // Установить дополнительные свойства для WordArt
                textEffectFormat.FontBold = true;
                textEffectFormat.FontItalic = false;
                textEffectFormat.FontSize = 24;

                Console.WriteLine("SetTextEffect method executed successfully with MsoPresetTextEffect.TextEffect10");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetTextEffect method: {ex.Message}");
            }

            // Сохранить результат
            workbook.Save("TextEffectFormatMethodSetTextEffectWithMsoPresetTextEffectDemo.xlsx");
        }
    }
}
```

### См. также

* enum [MsoPresetTextEffect](../../msopresettexteffect/)
* class [TextEffectFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)



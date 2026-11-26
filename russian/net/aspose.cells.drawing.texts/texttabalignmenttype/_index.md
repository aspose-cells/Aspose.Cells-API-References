---
title: "Перечисление TextTabAlignmentType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Aspose.Cells.Drawing.Texts.TextTabAlignmentType enum. Представляет типы выравнивания табуляций текста."
type: docs
url: /ru/net/aspose.cells.drawing.texts/texttabalignmenttype/
---
## TextTabAlignmentType enumeration

Представляет типы выравнивания табуляции текста.

```csharp
public enum TextTabAlignmentType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Center | `0` | Текст на этой табуляции выровнен по центру. |
| Decimal | `1` | На этой табуляции десятичные знаки выровнены. |
| Left | `2` | Текст на этой табуляции выровнен по левому краю. |
| Right | `3` | Текст на этой табуляции выровнен по правому краю. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextsClassTextTabAlignmentTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создайте текстовое поле для демонстрации выравниваний табуляций.
            int textBoxIndex = worksheet.TextBoxes.Add(0, 0, 400, 300);
            var textBox = worksheet.TextBoxes[textBoxIndex];
            var paragraph = textBox.TextBody.TextParagraphs[0];

            // Добавьте табуляции с различными типами выравнивания.
            paragraph.Stops.Add(TextTabAlignmentType.Left, 100);
            paragraph.Stops.Add(TextTabAlignmentType.Center, 200);
            paragraph.Stops.Add(TextTabAlignmentType.Right, 300);
            paragraph.Stops.Add(TextTabAlignmentType.Decimal, 400);

            // Установите текст для демонстрации всех типов выравнивания.
            textBox.Text = "Left\tCenter\tRight\tDecimal\n" +
                           "Data\tData\tData\t12.34\n" +
                           "More\tMore\tMore\t56.78";

            // Примените форматирование, чтобы сделать табуляции видимыми.
            textBox.Font.Size = 12;
            textBox.TextBody.TextParagraphs[0].AlignmentType = TextAlignmentType.Left;

            // Сохранить результат
            workbook.Save("TextTabAlignmentTypeDemo.xlsx");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)



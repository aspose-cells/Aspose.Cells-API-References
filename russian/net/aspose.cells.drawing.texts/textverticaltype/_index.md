---
title: "Перечисление TextVerticalType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.Drawing.Texts.TextVerticalType. Представляет тип направления текста"
type: docs
url: /ru/net/aspose.cells.drawing.texts/textverticaltype/
---
## TextVerticalType enumeration

Представляет прямой тип текста.

```csharp
public enum TextVerticalType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Vertical | `0` | Вертикальное отображение восточноазиатского текста. |
| Horizontal | `1` | Горизонтальный текст. |
| VerticalLeftToRight | `2` | Отображается вертикально, а текст течёт сверху вниз, затем СЛЕВА направо |
| Vertical90 | `3` | Каждая строка повернута на 90 градусов по часовой стрелке |
| Vertical270 | `4` | Каждая строка повернута на 270 градусов по часовой стрелке |
| Stacked | `5` | Определяет, является ли весь текст вертикальным |
| StackedRightToLeft | `6` | Указывает, что вертикальный WordArt должен отображаться справа налево, а не слева направо. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextVerticalTypeDemo
    {
        public static void TextVerticalTypeExample()
        {
            // Создание объекта Workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавление прямоугольной формы на лист
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 50, 100);

            // Получение доступа к настройкам выравнивания текста формы
            ShapeTextAlignment shapeTextAlignment = shape.TextBody.TextAlignment;

            // Установка вертикального типа текста в Horizontal
            shapeTextAlignment.TextVerticalType = TextVerticalType.Horizontal;

            // Установка других свойств для демонстрации
            shapeTextAlignment.IsTextWrapped = true;
            shapeTextAlignment.RotateTextWithShape = true;
            shapeTextAlignment.TextVerticalOverflow = TextOverflowType.Clip;
            shapeTextAlignment.TextHorizontalOverflow = TextOverflowType.Clip;
            shapeTextAlignment.RotationAngle = 90;
            shapeTextAlignment.IsLockedText = false;
            shapeTextAlignment.AutoSize = false;
            shapeTextAlignment.TextShapeType = AutoShapeType.TextBox;
            shapeTextAlignment.TopMarginPt = 2.0d;
            shapeTextAlignment.BottomMarginPt = 2.0d;
            shapeTextAlignment.LeftMarginPt = 2.0d;
            shapeTextAlignment.RightMarginPt = 2.0d;
            shapeTextAlignment.IsAutoMargin = true;
            shapeTextAlignment.NumberOfColumns = 1;

            // Сохранение книги
            workbook.Save("TextVerticalTypeExample.xlsx");

            return;
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)



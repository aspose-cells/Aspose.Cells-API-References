---
title: "Класс ShapeTextAlignment"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Drawing.Texts.ShapeTextAlignment. Представляет настройку выравнивания текста фигур"
type: docs
url: /ru/net/aspose.cells.drawing.texts/shapetextalignment/
---
## ShapeTextAlignment class

Представляет настройку выравнивания текста фигуры;

```csharp
public class ShapeTextAlignment
```

## Свойства

| Имя | Описание |
| --- | --- |
| [AutoSize](../../aspose.cells.drawing.texts/shapetextalignment/autosize/) { get; set; } | Указывает, автоматически ли размер формы регулируется в соответствии с её содержимым. |
| [BottomMarginPt](../../aspose.cells.drawing.texts/shapetextalignment/bottommarginpt/) { get; set; } | Возвращает нижний отступ в единицах Points |
| [IsAutoMargin](../../aspose.cells.drawing.texts/shapetextalignment/isautomargin/) { get; set; } | Указывает, является ли отступ текстовой рамки автоматическим. |
| [IsLockedText](../../aspose.cells.drawing.texts/shapetextalignment/islockedtext/) { get; set; } | Указывает, заблокирована ли фигура, когда лист защищён. |
| [IsTextWrapped](../../aspose.cells.drawing.texts/shapetextalignment/istextwrapped/) { get; set; } | Получает или задает тип переноса текста в фигуре, содержащей текст. |
| [LeftMarginPt](../../aspose.cells.drawing.texts/shapetextalignment/leftmarginpt/) { get; set; } | Возвращает левый отступ в единицах Points |
| [NumberOfColumns](../../aspose.cells.drawing.texts/shapetextalignment/numberofcolumns/) { get; set; } | Получает и задает количество столбцов текста в ограничивающем прямоугольнике. |
| [RightMarginPt](../../aspose.cells.drawing.texts/shapetextalignment/rightmarginpt/) { get; set; } | Возвращает правый отступ в единицах Points |
| [RotateTextWithShape](../../aspose.cells.drawing.texts/shapetextalignment/rotatetextwithshape/) { get; set; } | Указывает, вращается ли текст вместе с формой. |
| [RotationAngle](../../aspose.cells.drawing.texts/shapetextalignment/rotationangle/) { get; set; } | Получает и задает вращение фигуры. |
| [TextHorizontalOverflow](../../aspose.cells.drawing.texts/shapetextalignment/texthorizontaloverflow/) { get; set; } | Получает и задает тип горизонтального переполнения текста в текстовом поле. |
| [TextShapeType](../../aspose.cells.drawing.texts/shapetextalignment/textshapetype/) { get; set; } | Получает и задает тип трансформации текста. |
| [TextVerticalOverflow](../../aspose.cells.drawing.texts/shapetextalignment/textverticaloverflow/) { get; set; } | Получает и задает тип вертикального переполнения текста в текстовом поле. |
| [TextVerticalType](../../aspose.cells.drawing.texts/shapetextalignment/textverticaltype/) { get; set; } | Получает и задает направление текста. |
| [TopMarginPt](../../aspose.cells.drawing.texts/shapetextalignment/topmarginpt/) { get; set; } | Возвращает верхний отступ в единицах Points |

## Методы

| Имя | Описание |
| --- | --- |
| override [Equals](../../aspose.cells.drawing.texts/shapetextalignment/equals/)(object) | Определяет, имеет ли данный экземпляр то же значение, что и другой указанный объект `ShapeTextAlignment`. |
| override [GetHashCode](../../aspose.cells.drawing.texts/shapetextalignment/gethashcode/)() |  |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class ShapeTextAlignmentDemo
    {
        public static void ShapeTextAlignmentExample()
        {
            // Создание объекта Workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавление прямоугольной формы на лист
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 50, 100);

            // Доступ к объекту ShapeTextAlignment
            ShapeTextAlignment shapeTextAlignment = shape.TextBody.TextAlignment;

            // Установка свойств
            shapeTextAlignment.IsTextWrapped = true;
            shapeTextAlignment.RotateTextWithShape = true;
            shapeTextAlignment.TextVerticalOverflow = TextOverflowType.Clip;
            shapeTextAlignment.TextHorizontalOverflow = TextOverflowType.Clip;
            shapeTextAlignment.RotationAngle = 90;
            shapeTextAlignment.TextVerticalType = TextVerticalType.Horizontal;
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
            workbook.Save("ShapeTextAlignmentExample.xlsx");

            return;
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)



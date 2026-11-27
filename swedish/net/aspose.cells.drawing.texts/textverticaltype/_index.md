---
title: "Enum TextVerticalType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Drawing.Texts.TextVerticalType enum. Representerar den direkta texttypen"
type: docs
url: /sv/net/aspose.cells.drawing.texts/textverticaltype/
---
## TextVerticalType enumeration

Representerar den direkta texttypen.

```csharp
public enum TextVerticalType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Vertical | `0` | Östasiatisk vertikal visning. |
| Horizontal | `1` | Horisontell text. |
| VerticalLeftToRight | `2` | Visas vertikalt och texten flödar uppifrån och ner sedan VÄNSTER till HÖGER |
| Vertical90 | `3` | Varje rad är roterad 90 grader medurs |
| Vertical270 | `4` | Varje rad är roterad 270 grader medurs |
| Stacked | `5` | Avgör om all text är vertikal |
| StackedRightToLeft | `6` | Anger att vertikal WordArt ska visas från höger till vänster snarare än från vänster till höger. |

### Exempel

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
            // Instansiering av ett Workbook-objekt
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägger till en rektangelform i kalkylbladet
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 50, 100);

            // Åtkomst till textjusteringsinställningarna för formen
            ShapeTextAlignment shapeTextAlignment = shape.TextBody.TextAlignment;

            // Ställer in textens vertikala typ till Horisontell
            shapeTextAlignment.TextVerticalType = TextVerticalType.Horizontal;

            // Ställer in andra egenskaper för demonstration
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

            // Sparar arbetsboken
            workbook.Save("TextVerticalTypeExample.xlsx");

            return;
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)



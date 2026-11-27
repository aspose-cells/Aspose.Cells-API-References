---
title: "Klass ShapeTextAlignment"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Drawing.Texts.ShapeTextAlignment-klass. Representerar inställningen för formers textjustering"
type: docs
url: /sv/net/aspose.cells.drawing.texts/shapetextalignment/
---
## ShapeTextAlignment class

Representerar inställningen för figurens textjustering;

```csharp
public class ShapeTextAlignment
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [AutoSize](../../aspose.cells.drawing.texts/shapetextalignment/autosize/) { get; set; } | Anger om storleken på formen justeras automatiskt enligt dess innehåll. |
| [BottomMarginPt](../../aspose.cells.drawing.texts/shapetextalignment/bottommarginpt/) { get; set; } | Returnerar den nedre marginalen i enheten punkter |
| [IsAutoMargin](../../aspose.cells.drawing.texts/shapetextalignment/isautomargin/) { get; set; } | Anger om marginalen för textramen är automatisk. |
| [IsLockedText](../../aspose.cells.drawing.texts/shapetextalignment/islockedtext/) { get; set; } | Anger om formen är låst när kalkylbladet är skyddat. |
| [IsTextWrapped](../../aspose.cells.drawing.texts/shapetextalignment/istextwrapped/) { get; set; } | Hämtar eller anger den textomslutna typen för formen som innehåller text. |
| [LeftMarginPt](../../aspose.cells.drawing.texts/shapetextalignment/leftmarginpt/) { get; set; } | Returnerar den vänstra marginalen i enheten punkter |
| [NumberOfColumns](../../aspose.cells.drawing.texts/shapetextalignment/numberofcolumns/) { get; set; } | Hämtar och anger antalet kolumner med text i den avgränsande rektangeln. |
| [RightMarginPt](../../aspose.cells.drawing.texts/shapetextalignment/rightmarginpt/) { get; set; } | Returnerar den högra marginalen i enheten punkter |
| [RotateTextWithShape](../../aspose.cells.drawing.texts/shapetextalignment/rotatetextwithshape/) { get; set; } | Anger om text roteras med formen. |
| [RotationAngle](../../aspose.cells.drawing.texts/shapetextalignment/rotationangle/) { get; set; } | Hämtar och anger rotationen för formen. |
| [TextHorizontalOverflow](../../aspose.cells.drawing.texts/shapetextalignment/texthorizontaloverflow/) { get; set; } | Hämtar och anger den horisontella översvämningstypen för texten i textrutan. |
| [TextShapeType](../../aspose.cells.drawing.texts/shapetextalignment/textshapetype/) { get; set; } | Hämtar och anger transformeringstypen för text. |
| [TextVerticalOverflow](../../aspose.cells.drawing.texts/shapetextalignment/textverticaloverflow/) { get; set; } | Hämtar och anger den vertikala översvämningstypen för texten i textrutan. |
| [TextVerticalType](../../aspose.cells.drawing.texts/shapetextalignment/textverticaltype/) { get; set; } | Hämtar och anger textriktningen. |
| [TopMarginPt](../../aspose.cells.drawing.texts/shapetextalignment/topmarginpt/) { get; set; } | Returnerar den övre marginalen i enheten punkter |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| override [Equals](../../aspose.cells.drawing.texts/shapetextalignment/equals/)(object) | Bestämmer om detta objekt har samma värde som ett annat specificerat `ShapeTextAlignment`-objekt. |
| override [GetHashCode](../../aspose.cells.drawing.texts/shapetextalignment/gethashcode/)() |  |

### Exempel

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
            // Instansiering av ett Workbook-objekt
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägger till en rektangelform i kalkylbladet
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 50, 100);

            // Åtkomst till ShapeTextAlignment-objektet
            ShapeTextAlignment shapeTextAlignment = shape.TextBody.TextAlignment;

            // Ställa in egenskaper
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

            // Sparar arbetsboken
            workbook.Save("ShapeTextAlignmentExample.xlsx");

            return;
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)



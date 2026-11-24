---
title: "Klasse ShapeTextAlignment"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Drawing.Texts.ShapeTextAlignment Klasse. Stellt die Einstellung der Textausrichtung von Shapes dar"
type: docs
url: /de/net/aspose.cells.drawing.texts/shapetextalignment/
---
## ShapeTextAlignment class

Stellt die Einstellung der Textausrichtung einer Form dar;

```csharp
public class ShapeTextAlignment
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [AutoSize](../../aspose.cells.drawing.texts/shapetextalignment/autosize/) { get; set; } | Gibt an, ob die Größe der Form automatisch an ihren Inhalt angepasst wird. |
| [BottomMarginPt](../../aspose.cells.drawing.texts/shapetextalignment/bottommarginpt/) { get; set; } | Gibt den unteren Rand in Punkten zurück |
| [IsAutoMargin](../../aspose.cells.drawing.texts/shapetextalignment/isautomargin/) { get; set; } | Gibt an, ob der Rand des Textrahmens automatisch ist. |
| [IsLockedText](../../aspose.cells.drawing.texts/shapetextalignment/islockedtext/) { get; set; } | Gibt an, ob das Shape gesperrt ist, wenn das Arbeitsblatt geschützt ist. |
| [IsTextWrapped](../../aspose.cells.drawing.texts/shapetextalignment/istextwrapped/) { get; set; } | Liest oder setzt den Zeilenumbruchtyp des Shapes, das Text enthält. |
| [LeftMarginPt](../../aspose.cells.drawing.texts/shapetextalignment/leftmarginpt/) { get; set; } | Gibt den linken Rand in der Einheit Punkte zurück |
| [NumberOfColumns](../../aspose.cells.drawing.texts/shapetextalignment/numberofcolumns/) { get; set; } | Liest und setzt die Anzahl der Textspalten im Begrenzungsrechteck. |
| [RightMarginPt](../../aspose.cells.drawing.texts/shapetextalignment/rightmarginpt/) { get; set; } | Gibt den rechten Rand in der Einheit Punkte zurück |
| [RotateTextWithShape](../../aspose.cells.drawing.texts/shapetextalignment/rotatetextwithshape/) { get; set; } | Gibt an, ob Text mit einer Form rotiert wird |
| [RotationAngle](../../aspose.cells.drawing.texts/shapetextalignment/rotationangle/) { get; set; } | Liest und setzt die Drehung der Form. |
| [TextHorizontalOverflow](../../aspose.cells.drawing.texts/shapetextalignment/texthorizontaloverflow/) { get; set; } | Liest und setzt den horizontalen Überlauftyp des Textfelds. |
| [TextShapeType](../../aspose.cells.drawing.texts/shapetextalignment/textshapetype/) { get; set; } | Liest und setzt den Transformationstyp des Textes. |
| [TextVerticalOverflow](../../aspose.cells.drawing.texts/shapetextalignment/textverticaloverflow/) { get; set; } | Liest und setzt den vertikalen Überlauftyp des Textfelds. |
| [TextVerticalType](../../aspose.cells.drawing.texts/shapetextalignment/textverticaltype/) { get; set; } | Liest und setzt die Textausrichtung. |
| [TopMarginPt](../../aspose.cells.drawing.texts/shapetextalignment/topmarginpt/) { get; set; } | Gibt den oberen Rand in der Einheit Punkte zurück |

## Methoden

| Name | Beschreibung |
| --- | --- |
| override [Equals](../../aspose.cells.drawing.texts/shapetextalignment/equals/)(object) | Bestimmt, ob diese Instanz denselben Wert wie ein anderes angegebenes `ShapeTextAlignment`-Objekt hat. |
| override [GetHashCode](../../aspose.cells.drawing.texts/shapetextalignment/gethashcode/)() |  |

### Beispiele

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
            // Instanziieren eines Workbook-Objekts
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ein Rechteck-Shape zum Arbeitsblatt hinzufügen
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 50, 100);

            // Zugriff auf das ShapeTextAlignment-Objekt
            ShapeTextAlignment shapeTextAlignment = shape.TextBody.TextAlignment;

            // Eigenschaften festlegen
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

            // Speichern der Arbeitsmappe
            workbook.Save("ShapeTextAlignmentExample.xlsx");

            return;
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)



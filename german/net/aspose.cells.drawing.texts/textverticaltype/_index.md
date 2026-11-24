---
title: "Enum TextVerticalType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Drawing.Texts.TextVerticalType enum. Stellt den Textausrichtungstyp dar"
type: docs
url: /de/net/aspose.cells.drawing.texts/textverticaltype/
---
## TextVerticalType enumeration

Stellt den Textdirekttyp dar.

```csharp
public enum TextVerticalType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Vertical | `0` | Ostasiatische vertikale Anzeige. |
| Horizontal | `1` | Horizontaler Text. |
| VerticalLeftToRight | `2` | Vertikal angezeigt und der Text fließt von oben nach unten, dann VON LINKS NACH RECHTS |
| Vertical90 | `3` | Jede Zeile ist um 90 Grad im Uhrzeigersinn gedreht |
| Vertical270 | `4` | Jede Zeile ist um 270 Grad im Uhrzeigersinn gedreht |
| Stacked | `5` | Bestimmt, ob der gesamte Text vertikal ist |
| StackedRightToLeft | `6` | Gibt an, dass vertikales WordArt von rechts nach links statt von links nach rechts angezeigt werden soll. |

### Beispiele

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
            // Instanziieren eines Workbook-Objekts
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ein Rechteck-Shape zum Arbeitsblatt hinzufügen
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 50, 100);

            // Zugriff auf die Textausrichtungseinstellungen des Shapes
            ShapeTextAlignment shapeTextAlignment = shape.TextBody.TextAlignment;

            // Festlegen des vertikalen Texttyps auf Horizontal
            shapeTextAlignment.TextVerticalType = TextVerticalType.Horizontal;

            // Weitere Eigenschaften zum Demonstrationszweck festlegen
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

            // Speichern der Arbeitsmappe
            workbook.Save("TextVerticalTypeExample.xlsx");

            return;
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)



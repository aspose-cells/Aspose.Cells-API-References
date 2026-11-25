---
title: "Enum TextVerticalType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Drawing.Texts.TextVerticalType enum. Rappresenta il tipo di direzione del testo"
type: docs
url: /it/net/aspose.cells.drawing.texts/textverticaltype/
---
## TextVerticalType enumeration

Rappresenta il tipo di direzione del testo.

```csharp
public enum TextVerticalType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Vertical | `0` | Visualizzazione verticale dell'Asia orientale. |
| Horizontal | `1` | Testo orizzontale. |
| VerticalLeftToRight | `2` | Visualizzato verticalmente e il testo scorre dall'alto verso il basso poi DA SINISTRA A DESTRA |
| Vertical90 | `3` | Ogni riga è ruotata di 90 gradi in senso orario |
| Vertical270 | `4` | Ogni riga è ruotata di 270 gradi in senso orario |
| Stacked | `5` | Determina se tutto il testo è verticale |
| StackedRightToLeft | `6` | Specifica che il WordArt verticale deve essere mostrato da destra a sinistra anziché da sinistra a destra. |

### Esempi

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
            // Istanziare un oggetto Workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiunta di una forma rettangolare al foglio di lavoro
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 50, 100);

            // Accesso alle impostazioni di allineamento del testo della forma
            ShapeTextAlignment shapeTextAlignment = shape.TextBody.TextAlignment;

            // Impostazione del tipo verticale del testo su Orizzontale
            shapeTextAlignment.TextVerticalType = TextVerticalType.Horizontal;

            // Impostazione di altre proprietà per dimostrazione
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

            // Salvataggio della cartella di lavoro
            workbook.Save("TextVerticalTypeExample.xlsx");

            return;
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)



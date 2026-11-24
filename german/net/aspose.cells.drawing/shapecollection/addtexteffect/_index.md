---
title: "ShapeCollection.AddTextEffect"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ShapeCollection-Methode. Fügt ein WordArt-Objekt ein"
type: docs
url: /de/net/aspose.cells.drawing/shapecollection/addtexteffect/
---
## ShapeCollection.AddTextEffect method

Fügt ein WordArt-Objekt ein.

```csharp
public Shape AddTextEffect(MsoPresetTextEffect effect, string text, string fontName, int size, 
    bool fontBold, bool fontItalic, int topRow, int top, int leftColumn, int left, int height, 
    int width)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Effekt | MsoPresetTextEffect | Der mso-Voreinstellungstext-Effekttyp. |
| Text | String | Der WordArt-Text. |
| fontName | String | Der Schriftname. |
| Größe | Int32 | Die Schriftgröße |
| fontBold | Boolean | Gibt an, ob die Schrift fett ist. |
| fontItalic | Boolean | Gibt an, ob die Schrift kursiv ist. |
| topRow | Int32 | Index der oberen linken Zeile. |
| oben | Int32 | Stellt den vertikalen Versatz der Form von ihrer linken Zeile dar, in Pixel. |
| leftColumn | Int32 | Index der oberen linken Spalte. |
| links | Int32 | Stellt den horizontalen Versatz der Form von ihrer linken Spalte in Pixeln dar. |
| Höhe | Int32 | Stellt die Höhe der Form dar, in Pixeln. |
| Breite | Int32 | Stellt die Breite der Form in Pixeln dar. |

### Rückgabewert

Gibt ein Shape-Objekt zurück, das das neue WordArt-Objekt darstellt.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddTextEffectWithMsoPresetTextEffectStringStrinDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            ShapeCollection shapes = worksheet.Shapes;

            Shape wordArt = shapes.AddTextEffect(
                MsoPresetTextEffect.TextEffect10,
                "Sample WordArt",
                "Arial",
                18,
                false,
                false,
                3,
                0,
                3,
                0,
                200,
                50
            );

            workbook.Save("WordArtDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Shape](../../shape/)
* enum [MsoPresetTextEffect](../../msopresettexteffect/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)



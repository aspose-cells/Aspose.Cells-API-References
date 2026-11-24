---
title: "ShapeCollection.AddWordArt"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ShapeCollection-Methode. Fügt vordefiniertes WordArt seit Excel 2007 hinzu."
type: docs
url: /de/net/aspose.cells.drawing/shapecollection/addwordart/
---
## ShapeCollection.AddWordArt method

Fügt vordefiniertes WordArt seit Excel 2007 hinzu.

```csharp
public Shape AddWordArt(PresetWordArtStyle style, string text, int topRow, int top, int leftColumn, 
    int left, int height, int width)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Stil | PresetWordArtStyle | Der vordefinierte WordArt-Stil. |
| Text | String | Der Text. |
| topRow | Int32 | Index der oberen linken Zeile. |
| oben | Int32 | Stellt den vertikalen Versatz der Form von ihrer linken Zeile dar, in Pixel. |
| leftColumn | Int32 | Index der oberen linken Spalte. |
| links | Int32 | Stellt den horizontalen Versatz der Form von ihrer linken Spalte in Pixeln dar. |
| Höhe | Int32 | Stellt die Höhe der Form dar, in Pixeln. |
| Breite | Int32 | Stellt die Breite der Form in Pixeln dar. |

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddWordArtWithPresetWordArtStyleStringInt32IDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Rufe die Formensammlung ab
            ShapeCollection shapes = worksheet.Shapes;

            // Füge ein WordArt mit angegebenen Parametern hinzu
            Shape wordArt = shapes.AddWordArt(
                PresetWordArtStyle.WordArtStyle1, 
                "Sample WordArt", 
                10,  // left
                10,  // top
                200, // width
                50,  // height
                100, // rotation
                200  // z-order
            );

            // Speichere die Arbeitsmappe
            workbook.Save("WordArtDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Shape](../../shape/)
* enum [PresetWordArtStyle](../../presetwordartstyle/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)



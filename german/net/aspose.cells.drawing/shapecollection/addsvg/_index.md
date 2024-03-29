---
title: AddSvg
second_title: Aspose.Cells für .NET-API-Referenz
description: Fügt SVG-Bild hinzu.
type: docs
weight: 300
url: /de/net/aspose.cells.drawing/shapecollection/addsvg/
---
## ShapeCollection.AddSvg method

Fügt SVG-Bild hinzu.

```csharp
public Picture AddSvg(int upperLeftRow, int top, int upperLeftColumn, int left, int height, 
    int width, byte[] svgData, byte[] compatibleImageData)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| upperLeftRow | Int32 | Zeilenindex oben links. |
| top | Int32 | Stellt den vertikalen Versatz der Form von der linken Zeile in Pixeleinheiten dar. |
| upperLeftColumn | Int32 | Spaltenindex oben links. |
| left | Int32 | Der horizontale Versatz der Form von der linken Spalte in Pixeleinheiten. |
| height | Int32 | Die Höhe der Form in Pixeleinheiten. |
| width | Int32 | Die Breite der Form in Pixeleinheiten. |
| svgData | Byte[] | Die SVG-Bilddaten. |
| compatibleImageData | Byte[] | Konvertierte Bilddaten von svg, um mit Excel 2016 oder niedrigeren Versionen kompatibel zu sein. |

### Beispiele

```csharp

[C#]
// SVG hinzufügen
using (FileStream fs = new FileStream("image.svg", FileMode.Open))
{
    int len = (int)fs.Length;
    byte[] imageData = new byte[len];
    fs.Read(imageData, 0, len);
    Picture picture = shapes.AddSvg(4, 0, 5, 0, -1, -1, imageData, null);
}
```

### Siehe auch

* class [Picture](../../picture)
* class [ShapeCollection](../../shapecollection)
* namensraum [Aspose.Cells.Drawing](../../shapecollection)
* Montage [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->

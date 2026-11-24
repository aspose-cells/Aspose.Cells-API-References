---
title: "ShapeCollection.AddSvg"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ShapeCollection-Methode. Fügt ein svg-Bild hinzu"
type: docs
url: /de/net/aspose.cells.drawing/shapecollection/addsvg/
---
## ShapeCollection.AddSvg method

Fügt ein SVG-Bild hinzu.

```csharp
public Picture AddSvg(int topRow, int top, int leftColumn, int left, int height, int width, 
    byte[] svgData, byte[] compatibleImageData)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| topRow | Int32 | Index der oberen linken Zeile. |
| oben | Int32 | Stellt den vertikalen Versatz der Form von ihrer linken Zeile dar, in Pixel. |
| leftColumn | Int32 | Index der oberen linken Spalte. |
| links | Int32 | Der horizontale Versatz der Form von ihrer linken Spalte, in Pixel. |
| Höhe | Int32 | Die Höhe der Form, in Pixel. |
| Breite | Int32 | Die Breite der Form, in Pixel. |
| svgData | Byte[] | Die svg-Bilddaten. |
| compatibleImageData | Byte[] | Konvertierte Bilddaten von svg, um mit Excel 2016 oder älteren Versionen kompatibel zu sein. |

### Beispiele

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddSvgWithInt32Int32Int32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Aspose.Cells.Drawing.ShapeCollection shapes = worksheet.Shapes;

            // SVG-Datei laden
            using (FileStream fs = new FileStream("image.svg", FileMode.Open))
            {
                int len = (int)fs.Length;
                byte[] imageData = new byte[len];
                fs.Read(imageData, 0, len);
                
                // SVG zum Arbeitsblatt hinzufügen
                Aspose.Cells.Drawing.Picture picture = shapes.AddSvg(4, 0, 5, 0, -1, -1, imageData, null);
            }

            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [Picture](../../picture/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)



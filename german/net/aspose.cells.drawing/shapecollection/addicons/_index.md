---
title: "ShapeCollection.AddIcons"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ShapeCollection-Methode. Fügt ein svg-Bild hinzu"
type: docs
url: /de/net/aspose.cells.drawing/shapecollection/addicons/
---
## ShapeCollection.AddIcons method

Fügt ein SVG-Bild hinzu.

```csharp
public Picture AddIcons(int topRow, int top, int leftColumn, int left, int height, int width, 
    byte[] imageByteData, byte[] compatibleImageData)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| topRow | Int32 | Index der oberen linken Zeile. |
| oben | Int32 | Stellt den vertikalen Versatz der Form von ihrer linken Zeile dar, in Pixel. |
| leftColumn | Int32 | Index der oberen linken Spalte. |
| links | Int32 | Der horizontale Versatz der Form von ihrer linken Spalte, in Pixel. |
| Höhe | Int32 | Die Höhe der Form, in Pixel. |
| Breite | Int32 | Die Breite der Form, in Pixel. |
| imageByteData | Byte[] | Die Bild-Byte-Daten. |
| compatibleImageData | Byte[] | Konvertierte Bilddaten von svg, um mit Excel 2016 oder älteren Versionen kompatibel zu sein. |

### Beispiele

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddIconsWithInt32Int32Int32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            ShapeCollection shapes = worksheet.Shapes;

            // Erstellen Sie eine Beispiel-Icon-Datei (bei realer Verwendung würden Sie eine vorhandene Datei verwenden)
            string iconPath = "icon.svg";
            File.WriteAllText(iconPath, "<svg xmlns='http://www.w3.org/2000/svg' width='100' height='100'><circle cx='50' cy='50' r='40' fill='red'/></svg>");

            // Icon zum Arbeitsblatt hinzufügen
            using (FileStream fs = new FileStream(iconPath, FileMode.Open))
            {
                int len = (int)fs.Length;
                byte[] imageData = new byte[len];
                fs.Read(imageData, 0, len);
                Picture picture = shapes.AddIcons(4, 0, 5, 0, -1, -1, imageData, null);
            }

            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");

            // Aufräumen (optional)
            File.Delete(iconPath);
        }
    }
}
```

### Siehe auch

* class [Picture](../../picture/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)



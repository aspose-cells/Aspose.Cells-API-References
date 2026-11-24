---
title: "ShapeCollection.AddFreeFloatingShape"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ShapeCollection-Methode. Fügt der Arbeitsmappe eine frei schwebende Form hinzu. Gilt nur für Linien-/Bildformen"
type: docs
url: /de/net/aspose.cells.drawing/shapecollection/addfreefloatingshape/
---
## ShapeCollection.AddFreeFloatingShape method

Fügt eine frei schwebende Form zum Arbeitsblatt hinzu. Gilt nur für Linien-/Bildformen.

```csharp
public Shape AddFreeFloatingShape(MsoDrawingType type, int top, int left, int height, int width, 
    byte[] imageData, bool isOriginalSize)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Typ | MsoDrawingType | Der Formtyp. |
| oben | Int32 | Stellt den vertikalen Abstand der Form von der obersten Zeile der Arbeitsmappe dar, in Pixel. |
| links | Int32 | Stellt den horizontalen Abstand der Form von der linken Spalte der Arbeitsmappe dar, in Pixel. |
| Höhe | Int32 | Repräsentiert die Höhe von LineShape, in Pixel. |
| Breite | Int32 | Repräsentiert die Breite von LineShape, in Pixel. |
| imageData | Byte[] | Die Bilddaten, gelten nur für das Bild. |
| isOriginalSize | Boolean | Gibt an, ob die Form die Originalgröße verwendet, wenn die Form ein Bild ist. |

### Beispiele

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddFreeFloatingShapeWithMsoDrawingTypeInt32Int32Int32IDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            ShapeCollection shapes = worksheet.Shapes;

            // Eine Linienform hinzufügen
            Shape floatingShape_Line = shapes.AddFreeFloatingShape(
                MsoDrawingType.Line, 
                100, 100, 100, 50, 
                null, 
                false);

            // Füge eine Bildform hinzu (unter Verwendung von Beispiel-Bilddaten)
            byte[] imageData = null;
            try
            {
                using (FileStream fs = new FileStream("image.jpg", FileMode.Open))
                {
                    imageData = new byte[fs.Length];
                    fs.Read(imageData, 0, (int)fs.Length);
                }
            }
            catch
            {
                // Erstelle Dummy-Bilddaten, falls die Datei nicht gefunden wird
                imageData = new byte[100];
            }

            Shape floatingShape_Picture = shapes.AddFreeFloatingShape(
                MsoDrawingType.Picture, 
                200, 100, 100, 50, 
                imageData, 
                false);

            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [Shape](../../shape/)
* enum [MsoDrawingType](../../msodrawingtype/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)



---
title: "ShapeCollection.AddRectangle"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ShapeCollection-Methode. Fügt dem Arbeitsblatt ein RectangleShape hinzu"
type: docs
url: /de/net/aspose.cells.drawing/shapecollection/addrectangle/
---
## ShapeCollection.AddRectangle method

Fügt ein RectangleShape zum Arbeitsblatt hinzu.

```csharp
public RectangleShape AddRectangle(int topRow, int top, int leftColumn, int left, int height, 
    int width)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| topRow | Int32 | Index der oberen linken Zeile. |
| oben | Int32 | Stellt den vertikalen Versatz des RectangleShape von seiner linken Zeile in Pixeln dar. |
| leftColumn | Int32 | Index der oberen linken Spalte. |
| links | Int32 | Stellt den horizontalen Versatz von RectangleShape von seiner linken Spalte dar, in Pixel. |
| Höhe | Int32 | Stellt die Höhe von RectangleShape dar, in Pixel. |
| Breite | Int32 | Stellt die Breite von RectangleShape dar, in Pixel. |

### Rückgabewert

Ein RectangleShape-Objekt.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddRectangleWithInt32Int32Int32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügt ein Rechteck mit den angegebenen Parametern hinzu
            RectangleShape rectangleShape = worksheet.Shapes.AddRectangle(2, 0, 2, 0, 130, 130);

            // Speichere die Arbeitsmappe
            workbook.Save("RectangleShapeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [RectangleShape](../../rectangleshape/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)



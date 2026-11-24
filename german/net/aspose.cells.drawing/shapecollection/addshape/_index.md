---
title: "ShapeCollection.AddShape"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ShapeCollection-Methode. Fügt dem Arbeitsblatt eine Shape hinzu"
type: docs
url: /de/net/aspose.cells.drawing/shapecollection/addshape/
---
## ShapeCollection.AddShape method

Fügt ein Shape zum Arbeitsblatt hinzu.

```csharp
public Shape AddShape(MsoDrawingType type, int topRow, int top, int leftColumn, int left, 
    int height, int width)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Typ | MsoDrawingType | Mso-Zeichnungstyp. |
| topRow | Int32 | Index der oberen linken Zeile. |
| oben | Int32 | Stellt den vertikalen Versatz der Shape von ihrer linken Zeile dar, in Pixeln. |
| leftColumn | Int32 | Index der oberen linken Spalte. |
| links | Int32 | Stellt den horizontalen Versatz der Shape von ihrer linken Spalte dar, in Pixeln. |
| Höhe | Int32 | Stellt die Höhe der Shape dar, in Pixeln. |
| Breite | Int32 | Stellt die Breite der Shape dar, in Pixeln. |

### Rückgabewert

Ein Shape-Objekt.

### Hinweise

Der Typ darf nicht Chart/Comment/Picture/OleObject/Polygon/DialogBox sein

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddShapeWithMsoDrawingTypeInt32Int32Int32IDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            ShapeCollection shapes = worksheet.Shapes;
            Shape shape = shapes.AddShape(MsoDrawingType.Rectangle, 0, 0, 100, 100, 200, 50);
            
            Console.WriteLine("Shape added successfully.");
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



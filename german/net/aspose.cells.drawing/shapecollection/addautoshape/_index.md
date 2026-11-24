---
title: "ShapeCollection.AddAutoShape"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ShapeCollection-Methode. Fügt ein AutoShape zum Arbeitsblatt hinzu"
type: docs
url: /de/net/aspose.cells.drawing/shapecollection/addautoshape/
---
## ShapeCollection.AddAutoShape method

Fügt ein AutoShape zum Arbeitsblatt hinzu.

```csharp
public Shape AddAutoShape(AutoShapeType type, int topRow, int top, int leftColumn, int left, 
    int height, int width)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Typ | AutoShapeType | Auto-Formtyp. |
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
    public class ShapeCollectionMethodAddAutoShapeWithAutoShapeTypeInt32Int32Int32InDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            ShapeCollection shapes = worksheet.Shapes;
            Shape autoShape = shapes.AddAutoShape(AutoShapeType.Cube, 1, 0, 1, 0, 100, 50);
            
            workbook.Save("AutoShapeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Shape](../../shape/)
* enum [AutoShapeType](../../autoshapetype/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)



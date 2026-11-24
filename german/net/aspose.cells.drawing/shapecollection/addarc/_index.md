---
title: "ShapeCollection.AddArc"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ShapeCollection-Methode. Fügt ein ArcShape zum Arbeitsblatt hinzu"
type: docs
url: /de/net/aspose.cells.drawing/shapecollection/addarc/
---
## ShapeCollection.AddArc method

Fügt ein ArcShape zum Arbeitsblatt hinzu.

```csharp
public ArcShape AddArc(int topRow, int top, int leftColumn, int left, int height, int width)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| topRow | Int32 | Index der oberen linken Zeile. |
| oben | Int32 | Repräsentiert den vertikalen Versatz von ArcShape von seiner linken Zeile, in Pixel. |
| leftColumn | Int32 | Index der oberen linken Spalte. |
| links | Int32 | Repräsentiert den horizontalen Versatz von ArcShape von seiner linken Spalte, in Pixel. |
| Höhe | Int32 | Repräsentiert die Höhe von ArcShape, in Pixel. |
| Breite | Int32 | Repräsentiert die Breite von ArcShape, in Pixel. |

### Rückgabewert

Ein ArcShape-Objekt.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddArcWithInt32Int32Int32Int32Int32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            ShapeCollection shapes = worksheet.Shapes;
            ArcShape arcShape = shapes.AddArc(10, 10, 100, 50, 45, 180);
            
            workbook.Save("AddArcDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ArcShape](../../arcshape/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


